## Apartment Rental Management System
### Description
<p align="justify">
Apartment Rental Management System is based on searching the apartments available for rent in cities. The apartment owner updates details of the apartments available for rent and the customer is updated on these details such as area occupied, rent amount, location and so on. This system is best suitable for both owners as well as tenants and is also a best application in the city place. Tenants can easily search the suitable apartment with their preferred location and the rent amount. It also allows the tenants to pay their rent online. The Apartment Rental System helps to save a lot of time for both parties. Hence this system is best applicable for the above reasons making Apartment Rental an easy process through an online system.</p>

### Technology Used
* Front End - HTML, CSS, JavaScript
* Back End - Python Flask
* Database - MySql
### Requirements
The source code of this project is written in Python. So, You'll require the following to run this project
* Install libraries and dependencies listed in **requirements.txt**
```bash
pip install -r requirements.txt
```
* Install **MYSQL Workbench**
* Install **XAMPP** server
### How to Run the Project
1. Fork the repo and open the folder in your VSCode.
2. Copy all the sql commands listed in the **database** folder and run in on **MYSQL Workbench**.
3. Start the following two processes in **XAMPP** once it has been installed and loaded:
   * **Apache Webserver** - to serve HTTP requests.
   * **MySQL Server** - the database server.
4. Navigate to main.py file and run the file in VSCode.
5. Click on the link generated to run the project.

APTLY: Apartment Rental System Documentation

1. Introduction

This document provides an overview of the APTLY, a web application for managing apartment rentals. The system allows administrators to manage apartments, tenants, and rent payments, while tenants can view available apartments, rent units, and make online payments.

2. Project Overview

Purpose: To streamline apartment rental operations, improve efficiency, and enhance user experience for both administrators and tenants.
Key Features:
Admin Dashboard:
View apartment availability and occupancy statistics.
Manage tenant accounts (add, update, delete).
Add, update, and delete apartment listings.
View rent status and payment history.
Generate reports.
Tenant Portal:
View available apartments.
Rent apartments online.
Make online rent payments.
View rent history and receipts.
Security:
User authentication and authorization.
Password hashing for enhanced security.
Basic input validation to prevent common vulnerabilities.
3. Installation and Setup Guide

Prerequisites:

Python 3.x
Flask
Flask-MySQLdb (or mysqlclient)
MySQL Server
Virtual Environment (recommended)
Installation:

Create a virtual environment: python3 -m venv venv
Activate the environment: source venv/bin/activate1   
1.
github.com
github.com
Install dependencies: pip install -r requirements.txt (create a requirements.txt file with the necessary libraries)
Configure database connection in app.py with your MySQL credentials.
Create Database:

Create a MySQL database named apartmentRental.
Import the provided SQL script to create the necessary tables in the database.
Run Application:

Execute python app.py to start the development server.
4. User Manual

Admin:
Access the admin panel by navigating to /AdminLogin.
Login with the provided credentials.
Use the admin dashboard to manage apartments, tenants, and rent.
Tenant:
Access the tenant portal by navigating to /TenantLogin.
Register a new account or login with existing credentials.
Browse available apartments.
Rent an apartment and make online payments.
5. Technical Documentation

Code Structure:
The code is organized into routes, each handling specific functionalities.
Helper functions and classes can be used to improve code reusability and maintainability.
Database Design:
The database schema includes tables for tenants, apartments, rent, payments, and other relevant entities.
Security Measures:
Password hashing using werkzeug.security.generate_password_hash.
Basic input validation to prevent common vulnerabilities.
6. Code Review and Refactoring

Improvements:
Replace MySQLdb with mysqlclient for improved compatibility and security.
Implement more robust input validation and sanitization to prevent SQL injection and other attacks.
Enhance session management for better security.
Create a dedicated models.py file to define database models for better organization.
Implement unit tests to ensure code correctness and stability.
Consider using a more secure session management technique like storing session data in a database or using a secure cookie library.
7. Testing Documentation

Unit Tests:
Write unit tests for individual functions and modules to ensure their correctness.
Integration Tests:
Test the integration of different components of the application, such as database interactions, user authentication, and business logic.
User Acceptance Testing (UAT):
Conduct UAT with real users to gather feedback and identify any usability issues.
8. Challenges and Solutions

Challenge: Ensuring data security and preventing vulnerabilities.
Solution: Implemented password hashing, basic input validation, and will further enhance security measures.
Challenge: Handling complex business logic, such as rent calculations and payment processing.
Solution: The code includes a placeholder for a RENTUPDATE stored procedure to handle rent calculations and updates.
9. Future Improvements

Enhanced Security: Implement more advanced security measures, such as two-factor authentication, rate limiting, and intrusion detection.
Improved User Interface: Design a more user-friendly and visually appealing interface.
Mobile Responsiveness: Make the application responsive on mobile devices.
Advanced Features:
Add features like property search filters, online chat support, and tenant communication tools.
Integrate with payment gateways for seamless online payments.
Implement a more robust reporting system.
10. References and Resources

Flask documentation: https://flask.palletsprojects.com/en/2.3.x/
MySQL documentation: https://dev.mysql.com/doc/
Python documentation: https://docs.python.org/3/

