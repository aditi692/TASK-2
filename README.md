# TASK-2
# SQL Data Insertion and Handling Nulls
# E-Commerce example 
Task 2 – SQL Data Insertion & Null Handling (E-Commerce Example)
✨ Overview
This task involves working with an e-commerce-style database using SQL. The goal was to practice adding data, handling missing information (NULLs), and cleaning up dummy or test entries.

We used SQLiteStudio for creating and managing the database.

🧱 What Was Created
Two tables were designed:

1. Customers
This table stores customer details like name, email, phone number, and city.

If email or phone was missing, we used default placeholder values.

If the city wasn't provided, it was automatically set to "Unknown".

2. Orders
This table holds order details including order date, total amount, and status.

If order details like total amount or status were missing, we filled them with:

0 for missing amounts

'Pending' as the default status

A fixed date (2025-06-25) if the date was missing

💾 Data Handling Steps
Inserted sample data
Some entries were added with missing fields on purpose (like no email or city).

Handled missing values
Using UPDATE, we replaced NULL fields with meaningful defaults.
Example:

Empty email → not_provided@shop.com

Empty phone → 0000000000

Deleted test records
We removed:

The dummy user entry

Orders with no amount and default status
