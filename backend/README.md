# Spring Boot Backend

This is the backend service for the `my-app` portfolio project, built with Spring Boot and Hibernate.

## 🔧 Tech Stack

- Java 21
- Spring Boot 3.5.0
- Maven
- Spring Web
- Spring Data JPA
- H2 Database (for development)
- Lombok

## 📦 Project Structure

```
backend/
├── src/
│   ├── main/java/com/myapp/backend
│   │   ├── controller/       # REST controllers
│   │   ├── service/          # (To be added) Business logic
│   │   ├── model/            # (To be added) JPA entities
│   │   └── config/           # Global config (e.g., CORS)
│   └── resources/
│       └── application.properties
├── pom.xml
```

## 🚀 How to Run Locally

### 1. Prerequisites

- Java 21
- Maven
- IntelliJ or compatible IDE

### 2. Run the Application

```bash
cd backend
./mvnw spring-boot:run
```

Or run `BackendApplication.java` in your IDE.

### 3. Test API

Open browser or Postman:

```
GET http://localhost:8080/api/hello
```

Expected response:

```
Hello from Spring Boot!
```

## 🧪 Development Notes

- CORS is globally configured to allow React frontend (`localhost:3000`)
- Future plans:
  - Add database configuration and models
  - Add authentication (Spring Security or JWT)
  - Expose API for ML microservice
  - Deploy backend as Docker container
