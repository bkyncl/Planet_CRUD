# Planet CRUD App

## Overview

The **Planet CRUD App** is a simple PHP application that allows users to **Create**, **Read**, **Update**, and **Delete** (CRUD) planet data from a MySQL database. The application allows users to interact with planet records and includes user authentication, ensuring only authorized users can modify the data. The app also supports exporting the planet data to a PDF format.

## Features

- **CRUD Operations**: Add, update, delete, and view planet data.
- **User Authentication**: Secure login and registration for users.
- **Database Interaction**: MySQL database to store planet data.
- **PDF Export**: Export the planet data as a PDF.
- **Responsive**: Designed to work on both desktop and mobile devices.

## Requirements

Before running the app, ensure you have the following installed:

- **PHP**: Version 7.4 or higher.
- **MySQL**: Version 5.7 or higher.
- **XAMPP/WAMP or similar local server**: To run PHP and MySQL.

## Setup Instructions

Follow these steps to set up and run the Planet CRUD app locally:

### 1. Clone the Repository

If you haven't already, clone the repository to your local machine using Git:

git clone https://github.com/bkyncl/Planet_CRUD.git

### 2. Move Files to Local Server Directory

Move the `Planet_CRUD` folder to your local server’s root directory:

- For **XAMPP**: `C:\xampp\htdocs\Planet_CRUD\`
- For **WAMP**: `C:\wamp64\www\Planet_CRUD\`

### 3. Create Database and User

1. Open **phpMyAdmin** (usually at `http://localhost/phpmyadmin`).
2. Create a new database called `astronomy_db`.
3. Create a new MySQL user with the following credentials:
   - **Username**: `student1`
   - **Password**: `pass`
4. Grant the user full permissions on the `astronomy_db` database.

Alternatively, you can run these SQL queries in phpMyAdmin or via MySQL command line:

```sql
CREATE DATABASE astronomy_db;

CREATE USER 'student1'@'localhost' IDENTIFIED BY 'pass';

GRANT ALL PRIVILEGES ON astronomy_db.* TO 'student1'@'localhost';

FLUSH PRIVILEGES;

### 4. Start Your Local Server

- For **XAMPP**: Open the XAMPP Control Panel and start **Apache** and **MySQL**.
- For **WAMP**: Start WAMP and ensure the icon is green, indicating that both Apache and MySQL are running.

### 5. Access the App

In your browser, visit: http://localhost/Planet_CRUD/

### 6. Login and Use the App

- Login using the username **`student1`** and password **`pass`**.
- You can now create, read, update, delete, and export planet data to a PDF.