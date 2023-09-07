# Coffee Shop Database Project README

## Overview

Welcome to the Coffee Shop Database project, where I, as a Data Engineer, have been tasked with designing a robust relational database system for a New York-based coffee shop chain. This project aims to streamline operations and enhance data-driven decision-making as the company expands nationally by opening franchise locations. Here, I'll provide an overview of the project's objectives, the software used, data sources, and key tasks.

## Objectives

The main objectives of this project are:

- Design a relational database system for improved operational efficiencies.
- Consolidate data from various sources, including spreadsheets, CSV files, and databases.
- Normalize tables to adhere to second normal form (2NF).
- Define primary keys and relationships between tables.
- Create database objects, including tables, views, and materialized views.
- Export and import data across different relational database management systems (RDBMS).

## Software Used

In this project, I utilized the following RDBMS:

- PostgreSQL
- IBM Db2 Database
- MySQL

## Data Sources

The data used in this project is sourced from various locations:

1. Staff information from a spreadsheet at headquarters.
2. Sales outlet information from another spreadsheet at headquarters.
3. Sales data in CSV format from the POS system in sales outlets.
4. Customer data in CSV format from a custom Customer Relationship Management (CRM) system.
5. Product information from a supplier's database in spreadsheet format.

## Project Tasks

### Task 1: Identify Entities

Entities identified for the central database design include:

- Staff
- Sales Outlet
- Sales Transaction
- Customer
- Product

### Task 2: Identify Attributes

Attributes for the "Sales Transaction" entity include:

- Transaction ID
- Date
- Time
- Sales Outlet
- Staff
- Customer
- Product
- Quantity

### Task 3: Create an ERD

I used the pgAdmin ERD Tool to create an Entity Relationship Diagram (ERD) that includes tables like "Sales Transaction" and "Product" with their respective attributes.
![Task3A](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/69865222-4236-4619-b905-4a4d8f33fdf3)
![Task3B](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/22e3ad56-21d9-4f4b-a78e-93db4c770204)

### Task 4: Normalize Tables

I normalized tables to ensure they adhere to the second normal form (2NF). For example, I created a new table named "Sales Detail" to eliminate repeating rows in the sales transaction table.
![Task4A](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/b4533224-0be2-4f93-80eb-c63ac279d96f)
![Task4B](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/d5e3c159-c9b1-4503-8e9d-457832cb17b5)

### Task 5: Define Keys and Relationships

I defined primary keys for each table and established relationships between tables, such as sales detail to sales transaction.
![Task5A](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/e7d80f56-8c3b-4f79-9a51-ec241d42f077)
![Task5B](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/089bf23c-e395-4078-a0c6-cff64ded9931)

### Task 6: Create Database Objects

I generated SQL scripts from the ERD and executed them in pgAdmin to create the database schema. Sample data was loaded using provided SQL scripts.
![Task 6A](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/399313ed-c477-48c4-b1a7-cc57f07ae727)
![Task 6B](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/d14fccb4-2bc0-4e5e-8578-d3572058499b)

### Task 7: Create a View and Export Data

I created a view named "Staff Locations View" and exported the view data to a CSV file.
![Task7](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/0d707606-23a7-4e8a-9ff3-3227b68f1e95)

### Task 8: Create a Materialized View and Export Data

I created a materialized view named "Product Info M-View" and exported its data to a CSV file.
![Task8](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/7cf59374-57ba-4843-a491-291e512d06cf)

### Task 9: Import Data into a Db2 Database

I loaded staff location information into a Db2 database named "STAFF_LOCATIONS."
![Task9](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/1643c52e-fd5f-4746-acf7-b0c9e5eb9d1c)

### Task 10: Import Data into a MySQL Database
![Task10](https://github.com/delightez/CoffeeShop_DataOps/assets/56348397/de7ca792-4e8f-4e36-9870-024ae71437ab)

I loaded product information into a MySQL database named "coffee_shop_products."

Please note screenshots for each task are available in the project files.
.

