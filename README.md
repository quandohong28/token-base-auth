## Token Base Auth with Laravel and JWT

This is a simple project to demonstrate how to use JWT with Laravel.

## Installation

1. Clone the repository

2. Run `composer install`

3. Run `cp .env.example .env`

4. Run `php artisan key:generate`

5. Set your database credentials in `.env`

6. Run `php artisan jwt:secret`

7. Run `php artisan migrate --seed`

8. Run `php artisan serve`


## API List

### 1. Register User

```
POST /api/register

header: Content-Type: application/json

body:
{
    "name": "Test User",
    "email": "testuser@example.com",
    "password": "password",
    "password_confirmation": "password"
}
```

### 2. Login User

```
POST /api/login

header: Content-Type: application/json

body:
{
    "email": "testuser@example.com",
    "password": "password"
}
```
