# Laravel Livewire CRUD Example

This repository provides a simple CRUD application using Laravel Livewire. This example covers basic operations like creating, reading, updating, and deleting posts, demonstrating the power of Livewire to build dynamic interfaces without leaving the comfort of Laravel.

## Features

- Create, Read, Update, Delete (CRUD) operations for posts.
- Uses Livewire for dynamic and reactive UI components.
- Built with Laravel 11, but compatible with Laravel 6 to Laravel 11.

## Requirements

- PHP >= 8.0
- Composer
- Laravel 6.x, 7.x, 8.x, 9.x, 10.x, or 11.x

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/laravel-livewire-crud.git
   cd laravel-livewire-crud
2. **Install Laravel:**

- If you don't have Laravel installed, you can create a new Laravel project using the following command:

    ```bash
    composer create-project laravel/laravel livewire-crud
3. **Install Dependencies:**

- Navigate to your project directory and run the following command to install required dependencies:

    ```bash
    composer install
4. **Create Migration and Model:**

- Create the posts table migration and model:

    ```bash
    php artisan make:migration create_posts_table
    php artisan make:model Post

- Then, run the migration:
    ```bash
    php artisan migrate
5. **Install Livewire:**

    Install Livewire using Composer:

    ```bash
    composer require livewire/livewire
6. **Create Livewire Component:**

    Create a Livewire component for handling CRUD operations:
    ```bash
    php artisan make:livewire posts

**Usage**
**CRUD Operations**
- Create: Add a new post with a title and body.
- Read: View the list of all posts.
- Update: Edit an existing post.
- Delete: Remove a post.

**Running the Application**

- To run the application, use the following command:
    ```bash
    php artisan serve
- Then, open your browser and navigate to:
    ```bash
    http://localhost:8000/
You should see the Livewire-powered CRUD application.

**Blade Files**

- resources/views/livewire/posts.blade.php: Main listing view for posts.
- resources/views/livewire/create.blade.php: Form for creating a new post.
- resources/views/livewire/update.blade.php: Form for updating an existing post.
- resources/views/welcome.blade.php: Main application layout with Livewire integration.

**Customization**
You can customize the views, models, and components to fit your needs. For more advanced usage, refer to the Laravel Livewire documentation.
