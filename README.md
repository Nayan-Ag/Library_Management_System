# Library Management System

Welcome to the **Library Management System** repository! This project is a Java Swing application integrated with MySQL for managing library operations efficiently. It provides features such as login authentication, book management, staff management, and admin profile editing.

## 🚀 How to Run

To run this project on your system, follow these steps:

### Clone the Repository:
``bash
git clone https://github.com/your_username/library-management-system.git

### Set Up MySQL Database:
- Install MySQL on your system if not already installed.
- Create a new database named library.
- Import the `library.sql` file provided in the repository to set up the required tables and sample data.

### Open the Project in IDE:
- Open the project in your preferred Java IDE (e.g., IntelliJ IDEA, Eclipse).

### Configure MySQL Connection:
- Update the MySQL connection details in the `DBConnection.java` file to match your MySQL server configuration.

### Run the Application:
- Build and run the `LibraryManagementSystem.java` file to start the application.

### Login Credentials:
- Use the following credentials for logging in as an admin:
  - Username: admin
  - Password: admin

## 📋 Features

### Login Page
- Allows users to authenticate with their username and password.
- Directs users to the dashboard upon successful login.
- Displays an error message for invalid credentials.

### Dashboard
- Provides a user-friendly interface with seven options:
  - **Books Available**
  - **Add Book**
  - **Remove Book**
  - **Staff Details**
  - **Add Staff**
  - **Remove Staff**
  - **Edit Admin**

### Books Available
- Displays a table with all available books.
- Allows users to fetch book details from the local MySQL database.
- Provides a cancel button to exit the operation.

### Add Book
- Accepts input for Book ID, Category, Name, Author, and Copies.
- Checks if the book is already present in the database.
- Increments the number of copies if the book already exists, otherwise adds a new book.

### Remove Book
- Takes either Book ID or Book Name as input.
- Removes the book if found in the database; otherwise, displays a message indicating that the book is not present.

### Staff Details
- Fetches details of staff members from the staffs table.
- Displays staff information in a user-friendly format.

### Add Staff
- Accepts input for Staff ID, Name, and Contact.
- Adds a new staff member to the staffs table.

### Remove Staff
- Accepts Staff ID or Name as input.
- Removes the staff member if found in the staffs table; otherwise, displays a message indicating that the staff member is not present.

### Edit Admin
- Allows the admin to choose from parameters such as User ID, Name, Password, and Contact.
- Updates the selected parameter in the admin table based on the input provided.




# 💾 Using the Database

To use the MySQL database provided with this project, follow these steps:

### Install MySQL Server:

- If you haven't already installed MySQL Server on your system, download and install it from the [official MySQL website](https://dev.mysql.com/downloads/mysql/).

### Create a New Database:

- Once MySQL Server is installed, open MySQL Workbench or any MySQL client tool of your choice.

- Create a new database named `library` using the following SQL command:
``sql
- CREATE DATABASE library;

## Import Database Schema and Sample Data:

- In the MySQL client tool, navigate to the `library.sql` file provided in the repository.

- Execute the SQL script to create the necessary tables and populate them with sample data:
``sql

- SOURCE /path/to/library.sql;
- Replace /path/to/library.sql with the absolute path to the library.sql file on your system.

## Verify Database Setup:

- Once the SQL script is executed successfully, verify that the library database contains the following tables:

- admin table
- books table
- staffs table

## Update Database Connection Details:

- Open the DBConnection.java file in the project.

- Modify the connection details (such as hostname, port, username, and password) to match your MySQL server configuration.

## Run the Application:

- Follow the instructions provided in the previous section to run the Library Management System application.

## Login with Admin Credentials:

- Upon launching the application, use the following credentials to log in as an admin:

- Username: admin
- Password: admin

By following these steps, you can set up the MySQL database required for the Library Management System application and ensure seamless integration with the Java Swing interface.
