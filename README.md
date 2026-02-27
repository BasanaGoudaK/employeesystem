📌 Employee Management System

A RESTful Employee Management System built using Spring Boot, Spring Data JPA (Hibernate), and MySQL.
This application provides CRUD operations to manage employee records.

🚀 Features

Create Employee

View All Employees

View Employee by ID

Update Employee

Delete Employee

REST API architecture

Layered architecture (Controller → Service → Repository)

Database integration using JPA & Hibernate

Connection pooling using HikariCP

🛠️ Technologies Used

Java 17+

Spring Boot

Spring Data JPA

Hibernate

MySQL

Maven

Postman (for API testing)

📂 Project Structure
com.basu.employeesystem
│
├── controller
│     └── EmployeeController
│
├── service
│     └── EmployeeService
│
├── repository
│     └── EmployeeRepository
│
├── model
│     └── Employee
│
└── EmployeesystemApplication
⚙️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/your-username/employeesystem.git
cd employeesystem
2️⃣ Configure Database

Update application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/employeesystem
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
3️⃣ Run the Application
mvn spring-boot:run

OR run EmployeesystemApplication.java from your IDE.

Application will start at:

http://localhost:8080
📌 API Endpoints
🔹 Get All Employees
GET /api/employees
🔹 Get Employee by ID
GET /api/employees/{id}
🔹 Create Employee
POST /api/employees

Sample JSON:

{
  "firstName": "Basu",
  "lastName": "Sirwar",
  "email": "basu@gmail.com",
  "department": "IT",
  "salary": 50000
}
🔹 Update Employee
PUT /api/employees/{id}
🔹 Delete Employee
DELETE /api/employees/{id}
🧠 Architecture

The project follows a layered architecture:

Controller Layer → Handles HTTP requests

Service Layer → Contains business logic

Repository Layer → Communicates with database

Database Layer → MySQL

🔐 Future Improvements

Add DTO Layer

Add Global Exception Handling

Add Validation using @Valid

Add Swagger Documentation

Add JWT Authentication

Add Unit & Integration Testing

Add Pagination & Sorting

👨‍💻 Author

Basu Sirwar
Java Full Stack Developer

📄 License

This project is open-source and free to use for learning purposes.
