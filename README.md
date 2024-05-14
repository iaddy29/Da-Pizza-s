# Da-Pizza-s

# Restaurant Management System Installation Guide

## Introduction
This document provides instructions for setting up the Restaurant Management System on your local machine using MySQL and Python.

## Prerequisites
- Python installed on your system
- MySQL installed on your system
- Basic understanding of Python and MySQL

## Installation Steps
1. **Clone the Repository**: 
   - Clone the repository from [GitHub Repository Link](#).
   - Alternatively, you can download and extract the ZIP file.

2. **Install Dependencies**:
   - Make sure you have `mysql-connector-python` installed.
   - You can install it using pip:
     ```
     pip install mysql-connector-python
     ```

3. **Database Setup**:
   - Open MySQL and run the following commands to set up the database:
     ```sql
     CREATE DATABASE resturant;
     USE resturant;
     CREATE TABLE login_details (
         Username VARCHAR(20) UNIQUE NOT NULL,
         Password VARCHAR(20) UNIQUE NOT NULL,
         Designation VARCHAR(20)
     );
     INSERT INTO login_details VALUES ('owner', 'owner@123', 'owner');
     CREATE TABLE resturant_details (
         Details VARCHAR(30) NOT NULL,
         Value VARCHAR(50) NOT NULL
     );
     INSERT INTO resturant_details VALUES ('Phone no', '9987 9987');
     INSERT INTO resturant_details VALUES ('Address', 'Block-J, Saket, Khanpur, New Delhi');
     INSERT INTO resturant_details VALUES ('email', 'pizza_lovers@gmail.com');
     INSERT INTO resturant_details VALUES ('website', 'pizzalovers.com');
     -- Create other required tables and insert initial data as per your requirements.
     ```

4. **Run the Application**:
   - Run the Python script to start the application:
     ```
     python your_script_name.py
     ```

5. **Accessing the Application**:
   - Once the application is running, you can access it through the provided URL or by typing `localhost` in your browser's address bar.

