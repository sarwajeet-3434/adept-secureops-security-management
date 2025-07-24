# Adept SecureOps - Centralized Security & Management System

## 🚀 Project Overview

**Adept SecureOps** is a comprehensive full-stack Java web application designed for internal security operations, incident tracking, and client safety management for Adept Infrastructure. The system provides a centralized platform for managing security incidents, client information, training modules, and generating analytical reports.

## ✨ Features

### Core Features
- **User Authentication & Authorization** - Secure login with Spring Security and BCrypt
- **Client Management** - Complete CRUD operations for client information
- **Incident Tracking** - Log, track, and manage security incidents with response time monitoring
- **PDF Report Generation** - Export incident reports and analytics using iText
- **Training Module** - Manage security training programs and certifications
- **Dashboard Analytics** - Real-time charts and metrics for security operations
- **Email Notifications** - Automated alerts for incident submissions using JavaMailSender

### Advanced Features
- **Role-based Access Control** - Different access levels for admins, managers, and users
- **File Upload** - Support for incident evidence and training materials
- **Search & Filter** - Advanced filtering for incidents and clients
- **Data Export** - Multiple export formats (PDF, Excel, CSV)
- **Audit Trail** - Complete logging of all system activities

## 🛠️ Technology Stack

### Backend
- **Java 11+** - Core programming language
- **Spring Boot 2.7.x** - Application framework
- **Spring Security** - Authentication and authorization
- **Spring Data JPA** - Database operations
- **MySQL 8.0** - Primary database
- **Maven** - Dependency management
- **iText 7** - PDF generation
- **JavaMailSender** - Email notifications

### Frontend
- **Thymeleaf** - Server-side templating engine
- **Bootstrap 5** - CSS framework
- **Chart.js** - Data visualization
- **jQuery** - JavaScript library
- **Font Awesome** - Icons

### Development Tools
- **Spring Boot DevTools** - Hot reload during development
- **H2 Database** - In-memory database for testing
- **JUnit 5** - Unit testing framework
- **Postman** - API testing

## 📁 Project Structure

```
adept-secureops/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── adept/
│   │   │           └── secureops/
│   │   │               ├── AdeptSecureOpsApplication.java
│   │   │               ├── config/
│   │   │               │   ├── SecurityConfig.java
│   │   │               │   ├── EmailConfig.java
│   │   │               │   └── WebConfig.java
│   │   │               ├── controller/
│   │   │               │   ├── AuthController.java
│   │   │               │   ├── ClientController.java
│   │   │               │   ├── IncidentController.java
│   │   │               │   ├── DashboardController.java
│   │   │               │   ├── TrainingController.java
│   │   │               │   └── ReportController.java
│   │   │               ├── entity/
│   │   │               │   ├── User.java
│   │   │               │   ├── Client.java
│   │   │               │   ├── Incident.java
│   │   │               │   ├── Report.java
│   │   │               │   ├── Training.java
│   │   │               │   └── AuditLog.java
│   │   │               ├── repository/
│   │   │               │   ├── UserRepository.java
│   │   │               │   ├── ClientRepository.java
│   │   │               │   ├── IncidentRepository.java
│   │   │               │   ├── ReportRepository.java
│   │   │               │   ├── TrainingRepository.java
│   │   │               │   └── AuditLogRepository.java
│   │   │               ├── service/
│   │   │               │   ├── UserService.java
│   │   │               │   ├── ClientService.java
│   │   │               │   ├── IncidentService.java
│   │   │               │   ├── ReportService.java
│   │   │               │   ├── TrainingService.java
│   │   │               │   ├── EmailService.java
│   │   │               │   └── DashboardService.java
│   │   │               ├── utils/
│   │   │               │   ├── PDFGenerator.java
│   │   │               │   ├── EmailHelper.java
│   │   │               │   ├── FileUploadUtil.java
│   │   │               │   └── DateUtils.java
│   │   │               └── dto/
│   │   │                   ├── UserDTO.java
│   │   │                   ├── ClientDTO.java
│   │   │                   ├── IncidentDTO.java
│   │   │                   └── DashboardDTO.java
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── application-dev.properties
│   │       ├── application-prod.properties
│   │       ├── static/
│   │       │   ├── css/
│   │       │   │   └── dashboard.css
│   │       │   ├── js/
│   │       │   │   ├── dashboard.js
│   │       │   │   ├── charts.js
│   │       │   │   └── incidents.js
│   │       │   └── uploads/
│   │       ├── templates/
│   │       │   ├── auth/
│   │       │   │   ├── login.html
│   │       │   │   └── register.html
│   │       │   ├── dashboard/
│   │       │   │   └── index.html
│   │       │   ├── clients/
│   │       │   │   ├── list.html
│   │       │   │   ├── form.html
│   │       │   │   └── details.html
│   │       │   ├── incidents/
│   │       │   │   ├── list.html
│   │       │   │   ├── form.html
│   │       │   │   └── details.html
│   │       │   ├── training/
│   │       │   │   ├── list.html
│   │       │   │   └── form.html
│   │       │   ├── reports/
│   │       │   │   └── analytics.html
│   │       │   └── layout/
│   │       │       ├── base.html
│   │       │       └── sidebar.html
│   │       └── data.sql
│   └── test/
│       └── java/
│           └── com/
│               └── adept/
│                   └── secureops/
│                       ├── AdeptSecureOpsApplicationTests.java
│                       ├── controller/
│                       ├── service/
│                       └── repository/
├── docs/
│   ├── API_Documentation.md
│   ├── Database_Schema.sql
│   └── Postman_Collection.json
├── scripts/
│   ├── setup.sh
│   └── deploy.sh
├── pom.xml
├── README.md
└── .gitignore
```

## 🚀 Quick Start

### Prerequisites
- **Java 11 or higher** - [Download here](https://www.oracle.com/java/technologies/downloads/)
- **Maven 3.6+** - [Download here](https://maven.apache.org/download.cgi)
- **MySQL 8.0+** - [Download here](https://dev.mysql.com/downloads/mysql/)
- **Git** - [Download here](https://git-scm.com/downloads)

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/adept-secureops.git
   cd adept-secureops
   ```

2. **Set up MySQL Database**
   ```sql
   CREATE DATABASE adept_secureops;
   CREATE USER 'secureops_user'@'localhost' IDENTIFIED BY 'secureops_password';
   GRANT ALL PRIVILEGES ON adept_secureops.* TO 'secureops_user'@'localhost';
   FLUSH PRIVILEGES;
   ```

3. **Configure Application Properties**
   
   Update `src/main/resources/application.properties`:
   ```properties
   # Database Configuration
   spring.datasource.url=jdbc:mysql://localhost:3306/adept_secureops
   spring.datasource.username=secureops_user
   spring.datasource.password=secureops_password
   
   # Email Configuration (Update with your SMTP settings)
   spring.mail.host=smtp.gmail.com
   spring.mail.port=587
   spring.mail.username=your-email@gmail.com
   spring.mail.password=your-app-password
   ```

4. **Install Dependencies and Run**
   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

5. **Access the Application**
   - Open your browser and navigate to: `http://localhost:8080`
   - Default admin credentials: 
     - Username: `admin@adept.com`
     - Password: `admin123`

## 🔧 Development Setup

### Using IDE (IntelliJ IDEA/Eclipse)

1. **Import Project**
   - Open IDE → Import → Maven Project
   - Select the `pom.xml` file

2. **Configure Database**
   - Install MySQL and create database
   - Update `application-dev.properties` with your database credentials

3. **Run Application**
   - Right-click on `AdeptSecureOpsApplication.java`
   - Select "Run" or "Debug"

### Using Command Line

```bash
# Development mode with hot reload
mvn spring-boot:run -Dspring-boot.run.profiles=dev

# Production mode
mvn spring-boot:run -Dspring-boot.run.profiles=prod

# Run tests
mvn test

# Package application
mvn clean package
```

## 📊 API Documentation

### Authentication Endpoints
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `POST /api/auth/logout` - User logout

### Client Management
- `GET /api/clients` - Get all clients
- `GET /api/clients/{id}` - Get client by ID
- `POST /api/clients` - Create new client
- `PUT /api/clients/{id}` - Update client
- `DELETE /api/clients/{id}` - Delete client

### Incident Management
- `GET /api/incidents` - Get all incidents
- `GET /api/incidents/{id}` - Get incident by ID
- `POST /api/incidents` - Create new incident
- `PUT /api/incidents/{id}` - Update incident
- `DELETE /api/incidents/{id}` - Delete incident

### Dashboard Analytics
- `GET /api/dashboard/stats` - Get dashboard statistics
- `GET /api/dashboard/incidents-by-type` - Get incidents grouped by type
- `GET /api/dashboard/response-time` - Get average response time
- `GET /api/dashboard/monthly-trends` - Get monthly incident trends

### Reports
- `GET /api/reports/incidents/pdf` - Generate incident report PDF
- `GET /api/reports/clients/pdf` - Generate client report PDF
- `POST /api/reports/custom` - Generate custom report

## 🧪 Testing

### API Testing with Postman

1. **Import Collection**
   - Open Postman
   - Import `docs/Postman_Collection.json`

2. **Set Environment Variables**
   - Base URL: `http://localhost:8080`
   - Token: (obtained from login endpoint)

3. **Test Authentication**
   - Run login request first
   - Copy the JWT token for subsequent requests

### Unit Testing

```bash
# Run all tests
mvn test

# Run specific test class
mvn test -Dtest=UserServiceTest

# Run tests with coverage
mvn test jacoco:report
```

## 🚀 Deployment

### Local Deployment

1. **Build JAR file**
   ```bash
   mvn clean package
   ```

2. **Run JAR file**
   ```bash
   java -jar target/adept-secureops-1.0.0.jar
   ```

### Cloud Deployment (Railway)

1. **Connect to Railway**
   ```bash
   npm install -g @railway/cli
   railway login
   railway init
   ```

2. **Deploy**
   ```bash
   railway up
   ```

3. **Set Environment Variables**
   ```bash
   railway variables set SPRING_PROFILES_ACTIVE=prod
   railway variables set DATABASE_URL=your_database_url
   railway variables set MAIL_USERNAME=your_email
   railway variables set MAIL_PASSWORD=your_password
   ```

### Docker Deployment

1. **Build Docker Image**
   ```bash
   docker build -t adept-secureops .
   ```

2. **Run Container**
   ```bash
   docker run -p 8080:8080 adept-secureops
   ```

## 📈 Usage Guide

### Admin Dashboard
- Access comprehensive analytics and system statistics
- Manage users, clients, and incidents
- Generate and download reports
- Configure system settings

### Incident Management
- Log new security incidents with detailed information
- Track response times and resolution status
- Assign incidents to team members
- Upload evidence files and documentation

### Client Management
- Maintain client database with contact information
- Track client security assessments and compliance
- Generate client-specific reports
- Monitor client incident history

### Training Module
- Create and manage security training programs
- Track employee training completion
- Generate training certificates
- Schedule periodic training sessions

## 🔒 Security Features

- **Authentication**: JWT-based authentication with Spring Security
- **Authorization**: Role-based access control (ADMIN, MANAGER, USER)
- **Password Security**: BCrypt password hashing
- **SQL Injection Prevention**: JPA/Hibernate parameterized queries
- **CSRF Protection**: Built-in Spring Security CSRF protection
- **Session Management**: Secure session handling
- **Input Validation**: Comprehensive input validation and sanitization

## 🛠️ Configuration

### Database Configuration
```properties
# Primary Database
spring.datasource.url=jdbc:mysql://localhost:3306/adept_secureops
spring.datasource.username=secureops_user
spring.datasource.password=secureops_password
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# JPA Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```

### Email Configuration
```properties
# SMTP Configuration
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=your-email@gmail.com
spring.mail.password=your-app-password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true
```

### File Upload Configuration
```properties
# File Upload Settings
spring.servlet.multipart.max-file-size=10MB
spring.servlet.multipart.max-request-size=10MB
file.upload.dir=uploads/
```

## 📝 Sample Data

The application includes sample data for testing:
- **Users**: Admin, Manager, and regular users
- **Clients**: Sample client companies with contact information
- **Incidents**: Various types of security incidents
- **Training**: Sample training programs and certifications

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Support

For support and questions:
- Email: support@adeptinfrastructure.com
- Documentation: [Wiki](https://github.com/your-username/adept-secureops/wiki)
- Issues: [GitHub Issues](https://github.com/your-username/adept-secureops/issues)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Spring Boot Team for the excellent framework
- Bootstrap for the responsive UI components
- Chart.js for data visualization
- iText for PDF generation capabilities
- MySQL for reliable database management

---

**Adept SecureOps** - Securing your operations, one incident at a time. 🔒
