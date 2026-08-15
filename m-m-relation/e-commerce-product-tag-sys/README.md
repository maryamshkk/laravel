# Laravel Product & Tag Management System

A Laravel-based CRUD application for managing **Products and Tags** with a **Many-to-Many relationship** between them.

## Features

### Product Management

* Create products
* View all products
* View product details
* Edit products
* Delete products
* Product validation
* Assign multiple tags to a product
* Update product tags

### Tag Management

* Create tags
* View all tags
* View tag details
* Edit tags
* Delete tags
* Tag validation

## Product Fields

* `name`
* `description`
* `price`
* `stock`

## Tag Fields

* `name`

## Relationship

The project uses a **Many-to-Many relationship** between Products and Tags.

A product can have multiple tags, and a tag can belong to multiple products.

```text
Product
   ↕
Many-to-Many
   ↕
Tag
```

The relationship is handled using Laravel Eloquent:

```php
public function tags()
{
    return $this->belongsToMany(Tag::class);
}
```

The product-tag relationship is managed using Laravel's `sync()` method.

## Validation
Form inputs are validated using Laravel's built-in request validation before storing or updating data.

## CRUD Operations

| Resource | Create | Read | Update | Delete |
| -------- | ------ | ---- | ------ | ------ |
| Products | ✅      | ✅    | ✅      | ✅      |
| Tags     | ✅      | ✅    | ✅      | ✅      |

## Technologies

* PHP
* Laravel
* Laravel Eloquent ORM
* MySQL
* Blade Templates
* HTML
* Tailwind CSS

## Project Concepts Practiced

* Laravel Resource Controllers
* CRUD Operations
* Route Model Binding
* Eloquent Models
* Many-to-Many Relationships
* Pivot Table
* `belongsToMany()`
* `sync()`
* Form Validation
* Blade Views
* Database Relationships
* Mass Assignment
* Redirects and Flash Messages

## Project Structure

```text
app/
├── Http/
│   └── Controllers/
│       ├── ProductController.php
│       └── TagController.php
│
├── Models/
│   ├── Product.php
│   └── Tag.php
│
resources/
└── views/
    ├── products/
    └── tags/
```

## Purpose

This project was built to practice **Laravel CRUD operations, Eloquent relationships, form validation, resource controllers, and Many-to-Many database relationships** through a practical Product and Tag Management System.
