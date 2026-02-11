# 🚀 Laravel API Project

A RESTful API built with Laravel, designed to provide scalable and secure backend services.  
This project follows best practices for clean architecture, validation, authentication, and structured API responses.

---

## 📖 Overview

This Laravel API provides endpoints for managing resources such as customers, authentication, and other business logic components. It is structured following modern Laravel standards including:

- Form Request Validation
- API Resource Responses
- Token-based Authentication
- Clean Controller Architecture
- Versioned API routes

---

## 🛠️ Tech Stack

- **PHP 8+**
- **Laravel 10+**
- **MySQL**
- **Laravel Sanctum (for API Authentication)**
- **Composer**

---

## 📂 Project Structure

laravel-api/
│
├── app/
│ ├── Http/
│ │ ├── Controllers/
│ │ ├── Requests/
│ │ └── Resources/
│ ├── Models/
│
├── routes/
│ └── api.php
│
├── database/
│ ├── migrations/
│ └── seeders/
│
├── config/
├── .env
└── README.md


---

## ⚙️ Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/laravel-api.git
cd laravel-api
2️⃣ Install dependencies
composer install
3️⃣ Create environment file
cp .env.example .env
Configure your database inside .env.

Example:

DB_DATABASE=laravel_api
DB_USERNAME=root
DB_PASSWORD=
4️⃣ Generate application key
php artisan key:generate
5️⃣ Run migrations
php artisan migrate
6️⃣ Start the server
php artisan serve
Server will run at:

http://127.0.0.1:8000
🔐 Authentication
This API uses Laravel Sanctum for authentication.

To generate a token:

Send credentials to login endpoint

Receive token

Include token in headers:

Authorization: Bearer YOUR_TOKEN
📡 API Endpoints (Example)
Authentication
Method	Endpoint	Description
POST	/api/login	Login user
POST	/api/register	Register new user
Customers
Method	Endpoint	Description
GET	/api/v1/customers	Get all customers
POST	/api/v1/customers	Create customer
GET	/api/v1/customers/{id}	Get single customer
PUT	/api/v1/customers/{id}	Update customer
DELETE	/api/v1/customers/{id}	Delete customer
🧪 Testing with Postman
Obtain authentication token

Add token to Authorization header

Send requests to endpoints

🧱 Validation
All incoming requests are validated using Laravel Form Requests, ensuring:

Clean controllers

Secure data handling

Structured validation responses

📌 API Versioning
Routes are prefixed with:

/api/v1/
This allows future scalability (v2, v3, etc.)

🚧 Future Improvements
Swagger / OpenAPI documentation

Docker containerization

Automated tests (PHPUnit)

Role & Permission system

CI/CD pipeline integration

👨‍💻 Author
Sergio Fernandez
Full Stack Developer
📍 Mérida, Venezuela
📧 sergiofnzg@gmail.com
🔗 GitHub: https://github.com/sergiofnz
