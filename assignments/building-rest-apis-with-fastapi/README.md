# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI to manage a collection of books. Practice defining routes, validating request data, and returning appropriate HTTP status codes.

## 📝 Tasks

### 🛠️ Create the Books API

#### Description
Create a FastAPI application that stores a collection of books in memory. Each book should have an integer ID, a title, an author, and a publication year.

#### Requirements
Completed program should:

- Create and run a FastAPI application using Uvicorn
- Define a `GET /books` endpoint that returns all books as JSON
- Define a `GET /books/{book_id}` endpoint that returns the matching book
- Return a `404 Not Found` response when the requested book ID does not exist


### 🛠️ Add Book Creation and Validation

#### Description
Use a Pydantic model to define and validate the data required to create a book. Add an endpoint for adding books to the in-memory collection.

#### Requirements
Completed program should:

- Define a request model with title, author, and publication year fields
- Define a `POST /books` endpoint that adds a valid book and returns it as JSON
- Assign each new book a unique integer ID
- Reject requests with missing or invalid field values using FastAPI's validation response


### 🛠️ Complete and Test the CRUD API

#### Description
Add endpoints to update and delete books, then exercise every endpoint using FastAPI's interactive API documentation or automated tests.

#### Requirements
Completed program should:

- Define a `PUT /books/{book_id}` endpoint that updates an existing book
- Define a `DELETE /books/{book_id}` endpoint that removes an existing book
- Return a `404 Not Found` response when an update or delete targets an unknown book ID
- Verify listing, retrieving, creating, updating, and deleting books through `/docs` or automated tests
