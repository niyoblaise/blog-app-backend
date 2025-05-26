# Blog Platform Backend 🚀

A robust and secure backend system for a modern blog platform built with Spring Boot, featuring role-based authentication, 2FA support, and comprehensive content management capabilities.

## 🌟 Features

- **Secure Authentication**
  - JWT-based authentication
  - Two-factor authentication (2FA) support
  - Role-based access control (ADMIN, WRITER, READER)

- **Content Management**
  - CRUD operations for blog posts
  - Category management
  - Comment system
  - Post search functionality

- **User Management**
  - User registration and profile management
  - Role-based permissions
  - User activity tracking

- **Security Features**
  - Password encryption
  - JWT token validation
  - Rate limiting
  - CORS configuration

## 🛠️ Tech Stack

- Java 17
- Spring Boot 3.2.3
- Spring Security
- Spring Data JPA
- PostgreSQL
- Maven
- JWT for authentication
- Google Authenticator for 2FA

## 📋 Prerequisites

- Java 17 or higher
- Maven 3.6 or higher
- PostgreSQL 12 or higher
- IDE (IntelliJ IDEA recommended)

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd backend
   ```

2. **Configure Database**
   - Create a PostgreSQL database
   - Update `application.properties` with your database credentials:
     ```properties
     spring.datasource.url=jdbc:postgresql://localhost:5432/your_database
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     ```

3. **Build the project**
   ```bash
   mvn clean install
   ```

4. **Run the application**
   ```bash
   mvn spring-boot:run
   ```

The server will start on `http://localhost:8080`

## 🔧 Configuration

Key configuration properties in `application.properties`:

```properties
# Server Configuration
server.port=8080

# JWT Configuration
jwt.secret=your_jwt_secret
jwt.expiration=86400000

# Database Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

## 📚 API Documentation

The API documentation is available at:
- Swagger UI: `http://localhost:8080/swagger-ui.html`
- OpenAPI JSON: `http://localhost:8080/v3/api-docs`

## 🔐 Security

The application implements several security measures:
- JWT-based authentication
- Password encryption using BCrypt
- Role-based access control
- Two-factor authentication
- CORS configuration
- Rate limiting

## 🧪 Testing

Run the test suite:
```bash
mvn test
```

## 📦 Project Structure

```
src/main/java/com/blog
├── config/          # Configuration classes
├── controller/      # REST controllers
├── dto/            # Data Transfer Objects
├── entity/         # JPA entities
├── repository/     # Data repositories
├── security/       # Security configuration
├── service/        # Business logic
└── util/           # Utility classes
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Authors

- Niyonshuti Blaise - Initial work

## 🙏 Acknowledgments

- Spring Boot team for the amazing framework
- All contributors who have helped shape this project
