# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API using FastAPI to practice route creation, request/response modeling, and common HTTP status patterns. By the end of this assignment, you will be able to design and test basic API endpoints that return structured JSON data.

## 📝 Tasks

### 🛠️ API Setup and Health Check

#### Description
Create a new FastAPI project and implement a health check endpoint to verify that your API server is running correctly.

#### Requirements
Completed program should:

- Create a FastAPI app in a file named `main.py`.
- Add a `GET /health` endpoint that returns a JSON response with at least two keys: `status` and `service`.
- Start the app with Uvicorn and confirm the endpoint works in a browser or API client.
- Return HTTP status code `200` for successful health checks.

Example response:

```json
{
  "status": "ok",
  "service": "library-api"
}
```

### 🛠️ Build Book Resource Endpoints

#### Description
Implement core endpoints for a simple in-memory books API, including create, list, and fetch-by-id behavior.

#### Requirements
Completed program should:

- Define Pydantic models for request and response data.
- Implement `GET /books` to return all books.
- Implement `POST /books` to add a new book and return the created record.
- Implement `GET /books/{book_id}` to fetch one book by ID.
- Return `404` with a clear error message when a book ID does not exist.

Example API interaction:

```http
POST /books
Content-Type: application/json

{
  "title": "Deep Work",
  "author": "Cal Newport",
  "year": 2016
}
```

```json
{
  "id": 1,
  "title": "Deep Work",
  "author": "Cal Newport",
  "year": 2016
}
```
