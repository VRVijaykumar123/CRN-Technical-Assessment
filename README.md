# CRN-Technical-Assessment


# Product API

A RESTful Web API built using ASP.NET Core and Entity Framework Core for managing products. This project demonstrates CRUD operations, validation, clean architecture principles, and unit testing.

## Features

- Create, Read, Update, and Delete Products
- RESTful API endpoints
- Entity Framework Core with SQL Server
- Repository Pattern
- Dependency Injection
- Swagger/OpenAPI Documentation
- Global Exception Handling
- Unit Testing with xUnit
- Clean and Maintainable Code

## Tech Stack

- ASP.NET Core 8 Web API
- C#
- Entity Framework Core
- SQL Server
- xUnit
- Moq
- Swagger (Swashbuckle)

## Project Structure

```
ProductApi.sln
│
├── src
│   └── ProductApi
│
└── tests
    └── ProductApi.Tests
```

## Prerequisites

- .NET 8 SDK
- SQL Server
- Visual Studio 2022 or Visual Studio Code

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/your-username/ProductApi.git
cd ProductApi
```

### Configure Database

Update the connection string in:

```
appsettings.json
```

Example:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=.;Database=ProductDb;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

### Apply Migrations

```bash
dotnet ef database update
```

### Run the Application

```bash
dotnet run
```

The API will be available at:

```
https://localhost:5001
```

or

```
https://localhost:7xxx
```

depending on your launch settings.

## API Documentation

Swagger UI:

```
https://localhost:xxxx/swagger
```

## API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /api/products | Get all products |
| GET | /api/products/{id} | Get product by ID |
| POST | /api/products | Create a product |
| PUT | /api/products/{id} | Update a product |
| DELETE | /api/products/{id} | Delete a product |

## Running Tests

```bash
dotnet test
```

## Sample Product JSON

```json
{
  "name": "Laptop",
  "description": "Dell Inspiron",
  "price": 55000,
  "stock": 10
}
```

## Future Improvements

- JWT Authentication
- Pagination & Filtering
- Docker Support
- CI/CD Pipeline
- Logging with Serilog

## Author

**Vijay Kumar V R**

Email: vijaykumarvrwork@gmail.com

LinkedIn: https://linkedin.com/in/vijay-kumar-v-r-b311a5408
