# Bookstore Laravel Application

This project is a simple Bookstore web application built with Laravel. It allows users to manage a collection of books, including creating, viewing, updating, and deleting book records. The application demonstrates basic CRUD operations, search functionality, and uses Bootstrap for styling.

---

## 📺 Demo Video

<div align="center">
  
[![Book Store Laravel Demo](https://github.com/noobdevsam/book-store-laravel-project/blob/master/resources/Screenshot2025-05-22.png)](https://youtu.be/xfy8mjcSOgw)

</div>

> _Click the image above to watch the demo on YouTube!_


---

## Features
- List all books with pagination
- Search books by title or author
- Add new books (title, author, ISBN, stock, price)
- Edit existing book details
- View detailed information for each book
- Delete books

## Tech Stack
- **Backend:** Laravel 12 (PHP 8.2+)
- **Frontend:** Blade templates, Bootstrap 5
- **Database:** SQLite (default, can be changed)
- **Build Tools:** Vite, Tailwind CSS (optional)

## Getting Started

### Prerequisites
- PHP 8.2 or higher
- Composer
- Node.js and npm (for frontend assets)

### Installation
1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd bookstore
   ```
2. Install PHP dependencies:
   ```sh
   composer install
   ```
3. Install Node.js dependencies:
   ```sh
   npm install
   ```
4. Copy the example environment file and set your configuration:
   ```sh
   cp .env.example .env
   ```
5. Generate the application key:
   ```sh
   php artisan key:generate
   ```
6. Run database migrations and seeders:
   ```sh
   php artisan migrate --seed
   ```
7. Build frontend assets:
   ```sh
   npm run build
   ```
8. Start the development server:
   ```sh
   php artisan serve
   ```

Visit [http://localhost:8000/books](http://localhost:8000/books) to access the Bookstore app.

## Project Structure
- `app/Models/Book.php` - Book model
- `app/Http/Controllers/BookController.php` - Controller for book CRUD
- `resources/views/books/` - Blade templates for book views
- `database/migrations/` - Database schema
- `database/seeders/BookSeeder.php` - Seeds the database with sample books
- `routes/web.php` - Web routes

## Testing
Run tests with:
```sh
php artisan test
```

## License
This project is open-source and available under the [MIT license](LICENSE).
