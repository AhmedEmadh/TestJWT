# TestJWT

A simple project demonstrating **JWT (JSON Web Token) authentication** in .NET.

## 🚀 Features

- User login with JWT authentication

- Token generation with expiration

- Token validation middleware

- Secured API endpoints

## 🛠️ Tech Stack

- C# / .NET

- ASP.NET Core Web API

- JWT (System.IdentityModel.Tokens.Jwt)

## ▶️ Getting Started

### Prerequisites

- .NET SDK

- Visual Studio or VS Code

### Run the project

```bash
git clone https://github.com/AhmedEmadh/TestJWT.git
cd TestJWT
dotnet run
```

API available at:

```
https://localhost:5001
```

## 🔑 Example Usage

**Login (Get JWT)**  

`POST /api/auth/login`

```json
{
  "username": "testuser",
  "password": "password123"
}
```

Response:

```json
{
  "token": "eyJhbGciOiJIUzI1NiIsInR..."
}
```

**Access Protected Endpoint** 

`GET /api/secure/data` 
Header:

```
Authorization: Bearer <your_token_here>
```


