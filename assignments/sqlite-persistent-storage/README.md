# 📘 Assignment: SQLite and Persistent Storage

## 🎯 Objective

Extend a task-tracking API to store tasks in a SQLite database instead of keeping them only in memory. Learn to create a table, run SQL queries from Python, and verify that saved data is still available after the application restarts.

## 📝 Tasks

### 🛠️ Create a Tasks Database

#### Description
Use Python's built-in `sqlite3` module to create a SQLite database for a task-tracking application. Define a table that stores each task's ID, title, description, and completion status.

#### Requirements
Completed program should:

- Create or open a database file using `sqlite3`
- Create a `tasks` table with an integer primary key and columns for title, description, and completion status
- Create the table safely when the program starts, without deleting existing tasks
- Insert at least two sample tasks and retrieve them from the database


### 🛠️ Add Task Storage Operations

#### Description
Write Python functions that use SQL statements to create, read, update, and delete tasks in the database.

#### Requirements
Completed program should:

- Implement functions to add a task, list tasks, find a task by ID, update its completion status, and delete it
- Use SQL parameters rather than formatting user-provided values directly into SQL strings
- Commit changes that modify the database
- Handle a task ID that does not exist with a clear result or message


### 🛠️ Connect the API to SQLite

#### Description
Update the task-tracking API to use the database operations instead of an in-memory collection. Run the API, make changes to tasks, restart it, and confirm that the database preserved those changes.

#### Requirements
Completed program should:

- Use SQLite-backed operations for the API's task endpoints
- Return task data as JSON and report a not-found response when a requested task ID is missing
- Confirm that tasks added or updated through the API remain available after restarting the application
- Demonstrate that deleting a task removes it from subsequent API responses
