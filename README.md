# 🔐 AuthService

AuthService is a Spring Boot–based authentication and authorization microservice that provides secure login, JWT token generation, and refresh token management.

This service is designed to be scalable and easily integrated into a microservices architecture.

---

## 🚀 Features

- User Authentication
- JWT Token Generation
- Refresh Token Mechanism
- Password Encryption
- Secure REST APIs
- Global Exception Handling
- Layered Architecture (Controller → Service → DTO → Entity)

---

## 🛠 Tech Stack

- Java
- Spring Boot
- Spring Security
- JWT (JSON Web Token)
- Gradle
- REST APIs
- H2 / MySQL (if configured)

---

## 📂 Project Structure

```
AuthService
│── app
│   ├── src/main/java/org/example
│   │   ├── Controller
│   │   ├── Service
│   │   ├── entities
│   │   ├── request
│   │   ├── response
│   │   └── exception
│   │
│   └── src/main/resources
│       └── application.properties
│
├── build.gradle
├── settings.gradle
├── gradlew
└── gradlew.bat
```

---

## 🔐 Authentication Flow

1. User sends login request with credentials.
2. Credentials are validated.
3. JWT access token is generated.
4. Refresh token is generated and stored.
5. Access token is used to access protected APIs.
6. Refresh token can generate a new access token when expired.

---

## ▶️ How to Run the Project

### Using Gradle Wrapper

On Linux / Mac:
```bash
./gradlew bootRun
```

On Windows:
```bash
gradlew.bat bootRun
```

---

## 🧪 Running Tests

```bash
./gradlew test
```

---

## 📌 API Endpoints (Example)

- `POST /auth/login`
- `POST /auth/refresh`
- `GET /protected/resource`

*(Update endpoints if different in your project)*

---

## 🔒 Security Implementation

- Password hashing using secure encoder (e.g., BCrypt)
- Stateless authentication using JWT
- Refresh token validation
- Centralized exception handling

---

## 📈 Future Improvements

- Add Swagger documentation
- Dockerize the application
- Deploy to cloud (Render / AWS / Railway)
- Add role-based access control (RBAC)

---

## 👨‍💻 Author

**Ashutosh Dev**

GitHub: https://github.com/Phanto-Mbit