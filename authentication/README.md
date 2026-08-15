# Laravel Authentication System

A simple Laravel-based authentication system built to understand and implement the core authentication workflow in Laravel.

The project provides a complete user flow from registration and login to accessing a protected dashboard and managing profile information.

## Overview

This project demonstrates how Laravel handles user authentication, session management, protected routes, profile management, and secure password handling.

It was developed as a practical learning project to understand how controllers, models, middleware, validation, Blade views, and database operations work together in a Laravel application.

## Features

### Authentication

- User registration with form validation
- Secure password hashing
- User login with credential verification
- Session regeneration after successful login
- Logout functionality
- Authentication middleware for protected pages

### Dashboard

After successful authentication, users are redirected to a protected dashboard where their account information is displayed.

### Profile Management

Users can:

- View their profile
- Edit their profile information
- Change their password
- View account information such as name, email, and registration date

## Application Flow

```text
Registration
     ↓
User Validation
     ↓
Password Hashing
     ↓
Database
     ↓
Login
     ↓
Authentication
     ↓
Protected Dashboard
     ↓
Profile Management

```
### Project Structure

app/
├── Http/
│   ├── Controllers/
│   │   ├── AuthController.php
│   │   └── ProfileController.php
│   └── Middleware/

app/
└── Models/
    └── User.php

resources/
└── views/
    ├── layouts/
    ├── auth/
    ├── dashboard/
    └── profile/

routes/
└── web.php

### Tech Stack
-Laravel 13
-PHP 8.5
-MySQL
-Blade
-Tailwind CSS
-Eloquent ORM

## Key Laravel Concepts

The project provides practical experience with Laravel's authentication workflow, controllers, middleware, sessions, validation, Eloquent models, Blade layouts, route protection, and password hashing.

# Purpose

The main purpose of this project is to build a strong foundation in Laravel by implementing authentication and user profile functionality from scratch rather than relying on a pre-built authentication package.