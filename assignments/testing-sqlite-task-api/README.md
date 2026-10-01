# 📘 Assignment: Testing a SQLite Task API with pytest

## 🎯 Objective

Write automated tests for the SQLite-backed task API from the persistent storage assignment. Use pytest fixtures and FastAPI's test client to verify database operations and API behavior repeatably, without changing production data.

## 📝 Tasks

### 🛠️ Test the Database Operations

#### Description
Write pytest tests for the functions that create, retrieve, update, and delete tasks in SQLite. Use assertions to check returned values and database state, including what happens when a task ID does not exist.

#### Requirements
Completed program should:

- Test adding a task, listing tasks, and retrieving a task by ID
- Test updating and deleting an existing task
- Test the result of retrieving, updating, or deleting a task that does not exist
- Verify that a task remains stored after closing and reopening the database connection


### 🛠️ Test the API Endpoints

#### Description
Use FastAPI's `TestClient` to send requests to the task API directly from tests. Check both successful responses and errors, including request validation and unknown task IDs.

#### Requirements
Completed program should:

- Test the task listing, retrieval, creation, update, and deletion endpoints
- Check response status codes and JSON response data
- Check that invalid request data is rejected and unknown task IDs return the expected not-found response
- Run the tests without starting a separate Uvicorn server


### 🛠️ Isolate and Run the Test Suite

#### Description
Make every test use its own temporary SQLite database so tests do not depend on each other's data or alter the database used by the application. Adjust the storage code or app setup to accept a database path if needed.

#### Requirements
Completed program should:

- Use pytest's `tmp_path` fixture or an equivalent fixture to create a temporary database
- Ensure each test starts with a clean database and can be run independently
- Run the complete suite with `pytest -q` and confirm it passes more than once