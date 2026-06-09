# Online Quiz Application

## Overview

Online Quiz Application is a full-stack web application built using Spring Boot, Spring Security, Thymeleaf, and MySQL. The system provides a secure platform where users can register, verify their accounts using OTP, take quizzes with a timer, and view their results. Administrators can manage quiz questions through a dedicated dashboard.

---

## Features

### Authentication & Security

* User Registration
* Login using Username or Email
* Spring Security Authentication & Authorization
* Role-Based Access Control (Admin/User)
* Password Encryption using BCrypt
* Logout Functionality

### OTP Verification

* Email OTP Verification during Registration
* Forgot Password with OTP Verification
* OTP Expiration Timer
* OTP Resend Functionality

### Quiz Management

* Start Quiz
* Quiz Timer (10 Minutes)
* Automatic Submission when Time Expires
* Score Calculation
* Percentage Calculation
* Result Page with Performance Feedback

### Admin Features

* Add Quiz Questions
* Edit Quiz Questions
* Delete Quiz Questions
* Manage All Quizzes

### User Features

* Take Quiz
* View Results
* Profile Page
* Change Password
* Profile Picture Support
* Secure Session Handling

---

## Technologies Used

### Backend

* Java 21
* Spring Boot 4
* Spring Security
* Spring Data JPA
* Hibernate

### Frontend

* HTML5
* CSS3
* Thymeleaf

### Database

* MySQL

### Build Tool

* Maven

### Email Service

* JavaMailSender
* SMTP Email Integration

---

## Project Structure

src/main/java

├── config

│   ├── WebSecurityConfig

│   └── LoginSuccessHandler

├── controller

│   ├── AuthController

│   ├── QuizController

│   └── ProfileController

├── model

│   ├── User

│   └── Question

├── repository

│   ├── UserRepository

│   └── QuestionRepository

├── service

│   ├── QuizUserDetailsService

│   ├── QuestionsService

│   └── EmailService

src/main/resources

├── static

│   ├── css

│   ├── images

│   └── uploads

└── templates

```
├── login.html

├── register.html

├── home.html

├── quiz.html

├── result.html

└── profile.html
```

---

## Database Tables

### Users

| Field          | Type   |
| -------------- | ------ |
| id             | Long   |
| username       | String |
| password       | String |
| email          | String |
| role           | String |
| profilePicture | String |

### Questions

| Field         | Type   |
| ------------- | ------ |
| id            | Long   |
| questionText  | String |
| option1       | String |
| option2       | String |
| option3       | String |
| option4       | String |
| correctAnswer | String |

---

## Security Features

* BCrypt Password Encoding
* CSRF Protection
* Session Management
* Role-Based Authorization
* OTP Verification
* Secure Password Reset

---

## Future Improvements

* Quiz History
* User Statistics Dashboard
* Leaderboard
* Email Notifications
* Profile Picture Upload
* Change Email with OTP Verification
* REST API Version
* Docker Deployment

---

## Installation

### Clone Repository

git clone https://github.com/your-username/online-quiz.git

cd online-quiz

### Configure Database

Update application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/quizdb

spring.datasource.username=root

spring.datasource.password=your_password

### Configure Email

spring.mail.username=your_email

spring.mail.password=your_app_password

### Run Project

mvn clean install

mvn spring-boot:run

Application URL:

http://localhost:8080

---

## Screenshots

* Login Page
* Registration Page
* OTP Verification
* Home Dashboard
* Quiz Page
* Result Page
* Admin Quiz Management
* User Profile

(Add screenshots here)

---

## Author

YESHPAL SINGH

Java Full Stack Developer

Technologies:
Java | Spring Boot | Spring Security | MySQL | Thymeleaf | HTML | CSS

---

## Resume Highlights

This project demonstrates:

* Spring Boot Development
* Spring Security Implementation
* Role-Based Authentication
* Email OTP Verification
* Session Management
* CRUD Operations
* MVC Architecture
* Database Integration
* Full Stack Web Development
