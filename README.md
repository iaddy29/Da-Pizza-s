# Da-Pizza-s
Sure, here's a README file for the installation:

```markdown
# Restaurant Database Installation Guide

This guide will help you set up a MySQL database for a restaurant. The database includes tables for login details, restaurant details, IDs, employees, order items, order details, and the menu.

## Prerequisites

- MySQL Server
- Python 3.x
- `mysql-connector-python` package

## Steps

1. **Import the necessary modules**: Import the `mysql.connector` module in your Python script.

```python
import mysql.connector
```

2. **Connect to the MySQL Server**: Replace `'imaditya@123'` with your MySQL password.

```python
pas = 'imaditya@123'  # MySQL password
mydb = mysql.connector.connect(host='localhost', user='root', passwd=pas)
```

3. **Create a cursor object**: This object is used to execute SQL commands.

```python
mycursor = mydb.cursor()
```

4. **Create the database and tables**: Execute the SQL commands to create the database and tables. Make sure to replace the values in the `INSERT INTO` statements with your own data.

```python
mycursor.execute("create database resturant3")
mycursor.execute("use resturant")
mycursor.execute("create table login_details(Username VARCHAR(20) UNIQUE NOT null, Password Varchar(20) UNIQUE NOT NULL,Designation varchar(20))")
mycursor.execute("insert into login_details values('owner','owner@123','owner')")
...
```

5. **Commit the changes**: This will save all the changes made to the database.

```python
mydb.commit()
```

6. **Verify the installation**: Print a message to verify that the installation is completed.

```python
print("Installation Completed")
```

That's it! You have successfully set up your restaurant database.
```
