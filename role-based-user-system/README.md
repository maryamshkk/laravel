# Laravel Authentication & Role-Based User Management

A Laravel-based authentication and user management system with **role-based access control, admin dashboard, profile management, and RESTful User API**.

## Features

### 🔐 Authentication

* User registration
* User login
* User logout
* Session-based authentication
* Authentication validation
* Password hashing
* Automatic dashboard redirection based on user role

Customers are redirected to the normal dashboard, while administrators are redirected to the Admin Dashboard after login.

### 👥 Role-Based Authorization

The system supports two user roles:

* **Admin**
* **Customer**

Admins have access to the Admin Dashboard and User Management section, while customers have access to the normal user dashboard.

### 👨‍💼 Admin User Management

Admins can:

* View users
* Search users by name or email
* Create users
* Edit users
* Change user roles
* Update passwords
* Delete users
* Paginate users

User management includes search and pagination functionality.

### 👤 Profile Management

Authenticated users can:

* View their profile
* Update their name
* Upload a profile image
* Upload documents
* Change their password
* Logout

Profile images and uploaded files are stored using Laravel's public storage disk.

### 🌐 RESTful User API

The project also includes a User API with CRUD operations:

| Method    | Endpoint          | Description    |
| --------- | ----------------- | -------------- |
| GET       | `/api/users`      | Get all users  |
| GET       | `/api/users/{id}` | Get user by ID |
| POST      | `/api/users`      | Create user    |
| PUT/PATCH | `/api/users/{id}` | Update user    |
| DELETE    | `/api/users/{id}` | Delete user    |

The API returns JSON responses and validates user input before creating or updating records.

## Validation

Form inputs are validated using Laravel's built-in request validation, including name, email, password, role, image, and file validation.

## Security

* Passwords are hashed using Laravel's `Hash` facade / `bcrypt`
* Login uses Laravel's authentication system
* Sessions are regenerated after successful login
* Sessions are invalidated during logout
* Password change requires the current password
* Users cannot delete their own admin account

## Technologies

* PHP
* Laravel
* Laravel Eloquent ORM
* MySQL
* Blade Templates
* Tailwind CSS
* REST API
* JSON

## Laravel Concepts Practiced

* Authentication
* Authorization
* Role-Based Access Control
* CRUD Operations
* RESTful APIs
* Eloquent ORM
* Request Validation
* Route Model Binding
* Sessions
* Password Hashing
* File Uploads
* Laravel Storage
* Search
* Pagination
* Blade Templates
* Middleware

## Project Structure

```text
app/
├── Http/
│   └── Controllers/
│       ├── Admin/
│       │   └── UserController.php
│       ├── Api/
│       │   └── UserController.php
│       └── AuthController.php
│
├── Models/
│   └── User.php
│
resources/
└── views/
    ├── admin/
    │   ├── index.blade.php
    │   └── users/
    ├── auth/
    │   ├── login.blade.php
    │   └── register.blade.php
    ├── profile/
    ├── dashboard.blade.php
    └── layouts/
```

## Purpose

This project was developed to practice **Laravel authentication, role-based authorization, admin user management, RESTful APIs, CRUD operations, validation, sessions, password hashing, and file handling** in a complete web application.
