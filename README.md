# Set Up

Create environment file:

    cp .env.example .env

Edit .env file replacing database section with single line:

    DB_CONNECTION=sqlite

Create file for sqlite database:

    touch database/database.sqlite

Run migrations:

    php artisan migrate

Check tables have been created with sqlite command line or use PHPStorm to connect:

    sqlite3 database/database.sqlite

Serve application:

    php artisan serve

Check application is running on http://127.0.0.1:8000/
