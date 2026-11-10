# Digital Subsidy and Grant Administration Platform

An enterprise-grade, full-stack digital grant and subsidy management platform engineered to automate applicant eligibility evaluation, enforce role-based access control, and track fund disbursements transparently.

Developed as part of the **Infosys Springboard Virtual Internship 7.0**.

---

## Architecture & Directory Structure

```text
Digital-Subsidy-and-Grant-Administration-Platform/
├── backend/          # Java 17+, Spring Boot, Spring Security JWT, Hibernate, MySQL
│   ├── src/
│   └── pom.xml
├── frontend/         # React 18, Vite, Dual-theme UI (Light & Dark mode)
│   ├── src/
│   └── package.json
├── .gitignore
└── README.md

Key Features:-
Automated Eligibility Verification: Programmatic evaluation engine assessing applicant credentials and criteria rulesets.

Role-Based Access Control (RBAC): Token-based authentication (JWT) with distinct access levels for Applicants, Verification Officers, and Administrators.

Disbursement Lifecycle Tracking: End-to-end audit trail tracking applications through submission, document scrutiny, sanction, and fund release.

Responsive Dual-Theme Interface: Modern UI built with React featuring instant switching between Light and Dark (Night) modes.

Relational Integrity & Transactions: ACID-compliant data persistence using Spring Data JPA and Hibernate ORM over MySQL

Tech Stack
Layer                  Technologies

Backend	               Java 17+, Spring Boot, Spring Security, Spring Data JPA
frontend               React 18, Vite, Context API, Modern Modular CSS
Database               MySQL Server (subsidy_db)
Authentication         JSON Web Tokens (JWT), BCrypt Password Hashing
Build & Tools          Apache Maven, npm, Git

Getting Started
1. Database Configuration
Create a database in your local MySQL instance:

SQL
CREATE DATABASE subsidy_db;
Update your connection credentials in backend/src/main/resources/application.properties:

Properties
spring.datasource.url=jdbc:mysql://localhost:3306/subsidy_db?useSSL=false&serverTimezone=UTC
spring.datasource.username=YOUR_MYSQL_USERNAME
spring.datasource.password=YOUR_MYSQL_PASSWORD
spring.jpa.hibernate.ddl-auto=update

2. Run Backend Service
Bash
cd backend
mvn clean install
mvn spring-boot:run
Backend API service starts at http://localhost:8080

3. Run Frontend Application
Bash
cd frontend
npm install
npm run dev
Frontend dev server starts at http://localhost:5173

Author
Raushan Kumar

GitHub: @Raushan180-source