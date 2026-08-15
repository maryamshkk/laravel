# 📚 Library Management System

A Laravel-based **Library Management System** for managing books and their categories. The application provides a simple dashboard along with complete CRUD functionality for both **Books** and **Categories**.

## Features

### 📊 Dashboard

* Library overview dashboard
* Total categories count
* Total books count
* Quick navigation to Categories and Books management

### 📂 Category Management

* Create categories
* View all categories
* View category details
* Edit categories
* Delete categories

### 📖 Book Management

* Add new books
* View all books
* View book details
* Edit books
* Delete books
* Assign books to categories

### 🔗 Relationship

Books and Categories are connected using a **database relationship**, allowing each book to be associated with its relevant category.

## CRUD Operations

| Resource   | Create | Read | Update | Delete |
| ---------- | ------ | ---- | ------ | ------ |
| Categories | ✅      | ✅    | ✅      | ✅      |
| Books      | ✅      | ✅    | ✅      | ✅      |

## Validation

Form inputs are validated using Laravel's built-in request validation before storing or updating data.

## Dashboard

The dashboard displays:

* **Total Categories**
* **Total Books**
* Categories Management
* Books Management

## Technologies

* PHP
* Laravel
* Laravel Eloquent ORM
* MySQL
* Blade Templates
* Tailwind CSS

## Laravel Concepts Practiced

* CRUD Operations
* Resource Controllers
* Eloquent Models
* Database Migrations
* Eloquent Relationships
* Route Model Binding
* Form Validation
* Blade Templates
* Laravel Routing
* Tailwind CSS

## Project Structure

```text
app/
├── Http/
│   └── Controllers/
│       ├── BookController.php
│       └── CategoryController.php
│
├── Models/
│   ├── Book.php
│   └── Category.php
│
resources/
└── views/
    ├── books/
    ├── categories/
    └── dashboard.blade.php
```

## Purpose

This project was developed to practice **Laravel CRUD operations, database relationships, form validation, Eloquent ORM, Blade templating, and Tailwind CSS** by building a practical Library Management System.
