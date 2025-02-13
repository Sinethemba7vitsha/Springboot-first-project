User Login and Registration - Spring Boot

Overview

This project provides a user authentication system using Spring Boot. It includes secure login and registration functionalities, password hashing, and JWT-based authentication.

Features

User registration with validation

Secure password hashing with BCrypt

JWT-based authentication

Role-based access control

REST API endpoints for login and registration

Technologies Used

Spring Boot - Backend framework

Spring Security - Authentication and authorization

JWT (JSON Web Tokens) - Token-based authentication

MySQL/PostgreSQL - Database for storing user information

Hibernate (JPA) - ORM for database interaction

Lombok - Reducing boilerplate code

Installation

Clone the repository:

git clone https://github.com/your-username/user-auth-springboot.git
cd user-auth-springboot

Configure the database in application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/userdb
spring.datasource.username=root
spring.datasource.password=yourpassword

Build and run the application:

mvn clean install
mvn spring-boot:run

API Endpoints

Method

Endpoint

Description

POST

/api/auth/register

Register new user

POST

/api/auth/login

Authenticate user

GET

/api/users/me

Get user details

Security

Passwords are hashed using BCrypt.

JWT is used for user authentication and authorization.

Spring Security is configured to restrict access based on user roles.

Deployment

To package the application as a JAR:

mvn package

Run the JAR file:

java -jar target/user-auth-springboot.jar

Contribution

Feel free to contribute by submitting pull requests or opening issues for feature suggestions and bug fixes.

License

This project is licensed under the MIT License.
