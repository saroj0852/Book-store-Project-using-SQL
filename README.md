# 📚 Online Bookstore Management System (SQL Project)

## 📖 Overview
This project is a **database-driven Online Bookstore Management System** built using **MySQL**.  
It demonstrates how to design, implement, and query a relational database for managing books, customers, and orders.

The system covers **real-world bookstore operations**, including:
- Storing book details
- Managing customer information
- Tracking orders and inventory

---

## 🗂️ Project Structure
📂 Book-store-Project-using-SQL
┣ 📂 data/ # CSV data files
┃ ┣ Books.csv
┃ ┣ Customers.csv
┃ ┗ Orders.csv
┣ 📂 sql/
┃ ┣ schema.sql # Database schema (tables, constraints)
┃ ┣ import.sql # LOAD DATA INFILE commands for CSVs
┃ ┗ queries.sql # Sample SQL queries
┣ README.md # Project documentation

markdown
Copy code

---

## 🛠️ Features
- **Books Management**
  - Store book details (title, author, genre, year, price, stock).
- **Customer Management**
  - Maintain customer profiles with email, phone, city, country.
- **Orders Management**
  - Link customers with purchased books, track quantities and totals.
- **Data Import**
  - Bulk import data using `LOAD DATA INFILE` from CSV files.
- **SQL Queries**
  - Fetch available books by genre/author.
  - Find top-selling books.
  - Generate sales reports by customer/country.
  - Check inventory levels.

---

## 🏗️ Database Schema
### Tables:
- **Books**
  - `Book_ID`, `Title`, `Author`, `Genre`, `Published_Year`, `Price`, `Stock`
- **Customers**
  - `Customer_ID`, `Name`, `Email`, `Phone`, `City`, `Country`
- **Orders**
  - `Order_ID`, `Customer_ID`, `Book_ID`, `Quantity`, `Order_Date`

🔗 Relationships:
- One customer can place multiple orders.  
- One order contains one or more books.  

---

## ⚙️ Setup Instructions
1. **Clone the repo**
   ```bash
   git clone https://github.com/saroj0852/Book-store-Project-using-SQL.git
   cd Book-store-Project-using-SQL
