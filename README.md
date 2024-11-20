<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

 How to Set Up
How to Run the Bookstore Laravel Project
Follow these steps to set up and run the Bookstore locally:

1. Clone the Repository
git clone https://github.com/nazmulhasan77/bookstore_laravel_CRUD.git
2. Install Dependencies
Ensure you have Composer installed, then run:

composer install
3. Configure Environment
Copy the .env.example file to create a .env file:

cp .env.example .env
Open the .env file and set up your database configuration:

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password
4. Generate Application Key
Run the following command to generate a unique application key:

php artisan key:generate
5. Set Up the Database
Ensure the specified database exists. Then, run the migrations to set up the tables:

php artisan migrate
6. Seed the Database (Optional)
If the project includes data seeds, run:

php artisan db:seed
7. Start the Development Server
To run the project locally, start the Laravel development server:

php artisan serve
8. Access the Application
Open your browser and navigate to:

http://127.0.0.1:8000
Alternative: Run PHP Built-in Server
You can use the PHP built-in server instead of php artisan serve. Run the following command:

php -S localhost:8000 -t public
localhost:8000 specifies the host and port.
-t public sets the public directory as the document root (required for Laravel).
After following these steps, the Bookstore System should be running locally.

📂 Project Structure
├── app/
│   ├── Models/Book.php        # Book model
│   ├── Http/Controllers/BookController.php  # Controller
├── database/
│   ├── migrations/            # Database migrations
│   ├── seeders/BookSeeder.php # Seeder for test data
├── resources/views/books/     # Blade templates
├── routes/web.php             # Project routes
## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
