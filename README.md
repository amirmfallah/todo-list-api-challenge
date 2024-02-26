# Todo List RESTful API Challenge

## Introduction

In this challenge, you are tasked with creating a RESTful API for a Todo List application using Node.js, Express.js, PostgreSQL, and Prisma. The API will allow users to manage their todo items effectively, supporting operations such as creating, reading, updating, and deleting todos.

## Objective

Your goal is to design and implement a RESTful API that provides a seamless experience for managing todo items. Your API will interact with a PostgreSQL database to persist todo items and use Prisma as the ORM (Object-Relational Mapping) tool to simplify database operations.

## Requirements

### Technologies

- **Backend**: Node.js with Express.js framework
- **Database**: PostgreSQL
- **ORM**: Prisma

### API Endpoints

Your API should implement the following endpoints:

- `POST /todos`: Create a new todo item.
  - Request body should include: `title` (string, required), `description` (string, optional), `dueDate` (date, optional), `status` (string, optional, default 'pending').
- `GET /todos`: Retrieve a list of all todo items.
  - Support query parameters for filtering based on `status` and pagination (e.g., `limit`, `offset`).
- `GET /todos/:id`: Retrieve a single todo item by its ID.
- `PUT /todos/:id`: Update an existing todo item.
  - Request body may include any of the fields `title`, `description`, `dueDate`, `status`.
- `DELETE /todos/:id`: Delete a todo item by its ID.

### Data Model

Your todo items should at least contain the following fields:

- `id`: A unique identifier for the todo item.
- `title`: The title of the todo item.
- `description`: A longer description of the todo item.
- `dueDate`: The date by which the todo item should be completed.
- `status`: The current status of the todo item (e.g., 'pending', 'completed').

### Additional Features

- Implement validation for the request data and handle errors gracefully, returning meaningful error messages.
- Write middleware for logging requests to help with debugging and monitoring.
- Include a brief documentation or README file explaining how to set up and use your API.

## Evaluation Criteria

- **Functionality**: Your API endpoints must work as specified, correctly handling CRUD operations.
- **Code Quality**: Your code should be clean, well-organized, and properly commented.
- **Error Handling**: Your API should gracefully handle errors and return appropriate status codes and messages.
- **Documentation**: Your submission should include clear documentation or a README that explains how to set up and use your API.

## Submission Guidelines

- Push your code to a GitHub repository and provide the URL for review.
- Ensure your application is properly configured to connect to a PostgreSQL database.
- Include instructions for setting up the database and any required environment variables.

Good luck, and happy coding!
