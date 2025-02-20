Task Management System - Backend

Overview

This is the backend for the Task Management System, built using Spring Boot. It includes user authentication with JWT, AES encryption for security, and RESTful APIs for managing users and tasks.

Features

User Authentication: JWT-based authentication for secure access.

AES Encryption: Protects sensitive data.

Task Management: Create, update, delete, and retrieve tasks.

Spring Security: Ensures secure access to endpoints.

Spring Data JPA: Handles database interactions.

Tech Stack

Java 17

Spring Boot 3

Spring Security & JWT

Spring Data JPA

PostgreSQL/MySQL (Choose based on your setup)

Lombok (for reducing boilerplate code)

Prerequisites

Java 17 or later

Maven 3.8+

PostgreSQL or MySQL database

Installation & Setup

Clone the Repository:

git clone <repository-url>
cd backend

Configure Database:

Update application.properties or application.yml with your database credentials.

spring.datasource.url=jdbc:postgresql://localhost:5432/taskdb
spring.datasource.username=your_username
spring.datasource.password=your_password

Build & Run:

mvn clean install
mvn spring-boot:run

API Endpoints

Authentication

Login: POST /auth/login

Register: POST /auth/register

User Management

Get All Users: GET /users

Get User by ID: GET /users/{id}

Update User: PUT /users/{id}

Delete User: DELETE /users/{id}

Task Management

Create Task: POST /tasks

Get All Tasks: GET /tasks

Get Task by ID: GET /tasks/{id}

Update Task: PUT /tasks/{id}

Delete Task: DELETE /tasks/{id}

Security

JWT is used for authentication.

AES encryption is used for protecting sensitive data.

Secured endpoints require a Bearer token in the request header.

Environment Variables

JWT_SECRET: Secret key for JWT token generation.

AES_SECRET_KEY: Secret key for AES encryption.


