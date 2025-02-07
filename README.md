# CX Backend API

Backend API built with ASP.NET Core 7.0, featuring JWT authentication and Swagger documentation.

## Features

- JWT Authentication
- Swagger UI with Authorize button
- Secure endpoints
- Clean architecture

## Getting Started

1. Clone the repository
2. Install .NET 7.0 SDK
3. Run the application:
   ```bash
   dotnet run
   ```
4. Open Swagger UI: http://localhost:5074/docs

## API Endpoints

- POST `/api/auth/login` - Get JWT token
- GET `/api/secure` - Protected endpoint (requires JWT)

## Authentication

To authenticate:
1. Call `/api/auth/login` with:
   ```json
   {
       "username": "admin",
       "password": "password"
   }
   ```
2. Use the returned token in the Authorization header:
   ```
   Bearer [your-token]
   ```
