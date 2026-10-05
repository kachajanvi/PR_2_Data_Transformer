# PR_2_Data_Transformer

## Project Overview

Data Transformer is a SQL project developed to practice and demonstrate advanced SQL operations using a corporate data analysis system.

The project works with customer information, sales orders, and employee performance data. It demonstrates how SQL can be used to join, transform, analyze, and organize data for reporting and analysis.

## Author

**Janvi**

## Database

**Database Name:** `DataTransformerDB`

## Tables

The project contains three main tables:

### 1. Customers

Stores customer information.

| Column | Description |
|---|---|
| CustomerID | Unique ID of the customer |
| FirstName | Customer's first name |
| LastName | Customer's last name |
| Email | Customer email address |
| RegistrationDate | Date when the customer registered |

### 2. Orders

Stores sales order information.

| Column | Description |
|---|---|
| OrderID | Unique ID of the order |
| CustomerID | ID of the customer who placed the order |
| OrderDate | Date of the order |
| TotalAmount | Total amount of the order |

### 3. Employees

Stores employee information.

| Column | Description |
|---|---|
| EmployeeID | Unique ID of the employee |
| FirstName | Employee's first name |
| LastName | Employee's last name |
| Department | Employee department |
| HireDate | Employee joining date |
| Salary | Employee salary |

## SQL Concepts Used

This project demonstrates the following SQL concepts:

- Database creation and deletion
- Table creation
- Primary Key
- Foreign Key
- INSERT statements
- INNER JOIN
- LEFT JOIN
- RIGHT JOIN
- FULL OUTER JOIN using UNION
- Subqueries
- Aggregate functions
- Date functions
- String functions
- Window functions
- RANK()
- Running Total
- CASE expression
- Data formatting

## Queries Performed

The project performs 17 SQL tasks:

1. Retrieve orders with customer details using INNER JOIN.
2. Retrieve all customers and their orders using LEFT JOIN.
3. Retrieve all orders and corresponding customers using RIGHT JOIN.
4. Retrieve all customers and orders using UNION for FULL OUTER JOIN behavior.
5. Find customers who placed orders above the average order amount.
6. Find employees whose salary is above the average salary.
7. Extract the year and month from OrderDate.
8. Calculate the number of days between OrderDate and the current date.
9. Format OrderDate as DD-MM-YYYY.
10. Combine FirstName and LastName to create a full name.
11. Replace a part of a customer's name.
12. Convert FirstName to uppercase and LastName to lowercase.
13. Remove extra spaces from Email.
14. Calculate a running total of order amounts.
15. Rank orders according to TotalAmount.
16. Assign discounts according to the order amount.
17. Categorize employee salaries as High, Medium, or Low.

## Discount Rules

The discount is calculated using a CASE expression:

- More than 1000 → 10% Discount
- More than 500 → 5% Discount
- 500 or below → No Discount

## Salary Categories

Employee salaries are categorized as:

- 70000 or above → High
- 50000 to 69999 → Medium
- Below 50000 → Low

## Requirements

To run this project, you need:

- MySQL 8.0 or later
- MySQL-compatible SQL environment
- VS Code with a SQL/MySQL extension (optional)

## How to Run

1. Open MySQL or your SQL editor.
2. Open the SQL project file.
3. Run the complete SQL script.
4. The existing `DataTransformerDB` database will be removed if it exists.
5. A new `DataTransformerDB` database will be created.
6. The Customers, Orders, and Employees tables will be created.
7. Sample data will be inserted.
8. The 17 SQL queries can then be executed for analysis.

## Project Structure

```text
Data-Transformer/
│
├── DataTransformer.sql
└── README.md
