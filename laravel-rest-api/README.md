# Laravel User API

A RESTful User Management API built with **Laravel**. This API provides endpoints to manage users, including creating, retrieving, updating, and deleting users.

## Features

* Get all users
* Get a single user by ID
* Create a new user
* Update user information
* Delete a user
* Request validation
* Email uniqueness validation
* Password hashing using `bcrypt`
* JSON API responses
* HTTP status codes

## API Operations

| Method    | Endpoint          | Description         |
| --------- | ----------------- | ------------------- |
| GET       | `/api/users`      | Get all users       |
| GET       | `/api/users/{id}` | Get a specific user |
| POST      | `/api/users`      | Create a new user   |
| PUT/PATCH | `/api/users/{id}` | Update a user       |
| DELETE    | `/api/users/{id}` | Delete a user       |

## User Fields

* `name`
* `email`
* `password`

## Validation

### Create User

* `name` — required, minimum 3 characters
* `email` — required, valid email, must be unique
* `password` — required, minimum 6 characters

### Update User

* `name` — required, minimum 3 characters
* `password` — optional, minimum 6 characters

## Example Request

### POST `/api/users`

```json
{
    "name": "Maryam",
    "email": "maryam@example.com",
    "password": "password123"
}
```

### Response

```json
{
    "message": "user created successfully",
    "user": {
        "id": 1,
        "name": "Maryam",
        "email": "maryam@example.com"
    }
}
```

## Technologies

* PHP
* Laravel
* MySQL
* REST API
* JSON

## Project Purpose

This project was created to practice **Laravel REST APIs, CRUD operations, request validation, database interaction, and secure password handling**.
