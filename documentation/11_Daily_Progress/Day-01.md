# BankSphere-AI – Day 1 Progress

**Date:** 20 August 2026

## 1. Today's Goal

Set up the initial BankSphere-AI project structure, development environment, authentication microservice, and database connection.

## 2. Tasks Completed

### Project Setup

- Created the BankSphere-AI project folder.
- Created the backend folder.
- Created the documentation folder.
- Created the Project Overview documentation.

### GitHub

- Created GitHub repository for BankSphere-AI.

### Authentication Service

- Generated `auth-service` using Spring Initializr.
- Selected Java and Maven.
- Added Spring Boot dependencies required for the authentication service.
- Opened the project in IntelliJ IDEA.
- Verified that the Spring Boot application starts.

### Database Setup

- Installed MySQL.
- Installed MySQL Workbench.
- Created the database:

`banksphere_auth`

### Spring Boot Database Configuration

- Configured the MySQL database connection in `application.properties`.
- Connected the Auth Service with MySQL.
- Successfully started the Auth Service.

## 3. Error Encountered

Initially, the application failed with:

`Failed to configure a DataSource`

and:

`Failed to determine a suitable driver class`

### Reason

Spring Boot was using Spring Data JPA and MySQL dependencies, but the database connection properties had not yet been configured.

### Solution

Created the `banksphere_auth` MySQL database and configured the required datasource properties in `application.properties`.

## 4. What I Learned

Today I learned:

- How to create a Spring Boot project using Spring Initializr.
- How to open a Maven Spring Boot project in IntelliJ IDEA.
- Basic project structure of a Spring Boot application.
- How MySQL and MySQL Workbench are used.
- How to create a MySQL database.
- How Spring Boot connects to MySQL.
- The purpose of `application.properties`.
- Why datasource configuration is required when using JPA with MySQL.
- How to identify and fix a Spring Boot startup error.

## 5. Current Project Structure

```text
BankSphere-AI
├── backend
│   └── auth-service
│
└── documentation
    ├── 01_Project_Overview
    │   └── Project_Overview.md
    │
    └── 11_Daily_Progress
        └── Day-01.md