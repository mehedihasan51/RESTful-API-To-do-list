# To-Do List API


## Setup

1. Php Verson.
2. PHP 8.2.12,
3. Laravel 11,

## Setup Instructions

1. Clone the repository.
2. Run `composer install`.
3. Configure the `.env` file.
4. Run `php artisan migrate`.
5. Run `php artisan serve`.

## Configure the `.env` file

1. DB_CONNECTION=mysql
2. DB_HOST=127.0.0.1
3. DB_PORT=3306
4. DB_DATABASE=ToDo-Api
5. DB_USERNAME=root
6. DB_PASSWORD=

## Generate an Application Key

1. php artisan key:generate

## API Endpoints

- **Create Task:** POST `/api/tasks`
  - Request Body: `{ "title": "string", "description": "string" }`
  - Response: `201 Created`
- **Read Tasks:** GET `/api/tasks`
  - Response: `200 OK`
- **Read Single Task:** GET `/api/tasks/{id}`
  - Response: `200 OK`
- **Update Task:** PUT `/api/tasks/{id}`
  - Request Body: `{ "title": "string", "description": "string", "is_completed": "boolean" }`
  - Response: `200 OK`
- **Delete Task:** DELETE `/api/tasks/{id}`
  - Response: `204 No Content`

## Testing

- Run `php artisan test` to execute the tests.
