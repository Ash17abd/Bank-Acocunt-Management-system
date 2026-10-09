# 🏦 Bank Account Management System

A **DBMS-based Bank Account Management System** developed to manage customer accounts, banking transactions, beneficiaries, loans, savings, and account information efficiently.

The project demonstrates the practical implementation of **Database Management System concepts** using SQL.

---

## 📌 Project Overview

The Bank Account Management System provides a structured way to store and manage banking information in a database.

It allows users to:

* Create and manage bank accounts
* Deposit and withdraw money
* Transfer money between accounts
* Manage beneficiaries
* View transaction history
* Check account balance
* Manage savings goals
* Analyze spending
* Check loan eligibility
* Calculate EMI
* Manage customer information securely

---

## 🎯 Objectives

* To design and implement a relational database for banking operations.
* To understand database design and relationships.
* To perform CRUD operations using SQL.
* To maintain transaction records accurately.
* To apply DBMS concepts such as **Primary Key, Foreign Key, Constraints, Joins, Normalization, Views, and Aggregate Functions**.
* To provide an organized and efficient banking data management system.

---

## 🛠️ Technologies Used

| Technology         | Purpose                             |
| ------------------ | ----------------------------------- |
| SQL                | Database implementation             |
| DBMS               | Data storage and management         |
| MySQL / SQL Server | Database execution                  |
| GitHub             | Version control and project hosting |
| C++                | Optional application interface      |

---

## 🗄️ Database Modules

### 1. Customer Management

Stores customer details such as:

* Customer ID
* Name
* Phone Number
* Email
* Address

### 2. Account Management

Stores:

* Account Number
* Account Type
* Balance
* PIN
* Monthly Income
* Account Status

### 3. Transaction Management

Supports:

* Deposit
* Withdrawal
* Money Transfer
* Transaction History

### 4. Beneficiary Management

Stores beneficiary details required for account-to-account transfers.

### 5. Loan Management

Provides:

* Loan eligibility checking
* Loan amount
* Interest rate
* EMI calculation
* Loan status

### 6. Savings Management

Tracks:

* Savings goal
* Savings amount
* Progress towards savings target

### 7. Spending Analysis

Maintains spending information and helps analyze total expenses.

---

## 🧩 Database Concepts Used

This project demonstrates the following DBMS concepts:

* Primary Keys
* Foreign Keys
* Candidate Keys
* Constraints
* `CREATE TABLE`
* `INSERT`
* `UPDATE`
* `DELETE`
* `SELECT`
* `WHERE`
* `ORDER BY`
* `GROUP BY`
* Aggregate Functions
* Joins
* Subqueries
* Views
* Transactions
* Normalization
* Referential Integrity

---

## 📊 Example Database Structure

```text
CUSTOMER
   |
   | 1 : N
   ↓
ACCOUNT
   |
   | 1 : N
   ↓
TRANSACTION

ACCOUNT
   |
   | 1 : N
   ↓
BENEFICIARY

ACCOUNT
   |
   | 1 : N
   ↓
LOAN

ACCOUNT
   |
   | 1 : 1
   ↓
SAVINGS
```

---

## 🗃️ Main Tables

| Table         | Description                                     |
| ------------- | ----------------------------------------------- |
| `Customer`    | Stores customer information                     |
| `Account`     | Stores bank account details                     |
| `Transaction` | Stores deposit, withdrawal and transfer records |
| `Beneficiary` | Stores beneficiary information                  |
| `Loan`        | Stores loan details                             |
| `Savings`     | Stores savings goals and amounts                |

---

## 💻 Sample SQL Query

### Display Account Details

```sql
SELECT 
    account_no,
    name,
    balance,
    monthly_income
FROM Account;
```

### Find Accounts With Balance Greater Than ₹50,000

```sql
SELECT account_no, name, balance
FROM Account
WHERE balance > 50000;
```

### Calculate Total Balance

```sql
SELECT SUM(balance) AS total_balance
FROM Account;
```

### Display Transaction History

```sql
SELECT *
FROM Transaction
ORDER BY transaction_date DESC;
```

---

## 🔐 Security Features

* PIN-based account authentication
* Input validation
* Account status management
* Transaction verification
* Restricted access to account information

> **Note:** This project is an academic DBMS project and should not be used for real banking operations.

---

## 🚀 How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/bank-account-management-system.git
```

### Step 2: Open the SQL File

Open the SQL script using your preferred DBMS such as:

* MySQL Workbench
* SQL Server Management Studio
* Oracle SQL Developer

### Step 3: Create the Database

```sql
CREATE DATABASE BankManagement;
```

### Step 4: Select the Database

```sql
USE BankManagement;
```

### Step 5: Execute the SQL Script

Run the table creation, insertion, and query commands provided in the project files.

---

## 📁 Project Structure

```text
Bank-Account-Management-System/
│
├── README.md
├── database/
│   ├── create_tables.sql
│   ├── insert_data.sql
│   └── queries.sql
│
├── src/
│   └── bank_management.cpp
│
├── documentation/
│   └── project_report.pdf
│
└── screenshots/
    ├── login.png
    ├── dashboard.png
    └── transactions.png
```

---

## 👥 Team Members

* **Ashwin**
* **karthik**
* **mani lakshmi sri**
* **saida**

---

## 🎓 Academic Project

**Project:** Bank Account Management System
**Domain:** Database Management System
**Language:** SQL / C++
**Purpose:** Academic / Educational Project

---

## 🔮 Future Enhancements

* Online banking interface
* Mobile application
* OTP authentication
* Email/SMS transaction notifications
* Advanced fraud detection
* Real-time transaction monitoring
* Cloud database integration
* Role-based access control

---

## ⭐ Conclusion

The **Bank Account Management System** demonstrates how DBMS concepts can be applied to a real-world banking scenario. The system organizes customer, account, transaction, loan, beneficiary, and savings information while maintaining data consistency and integrity.

---

## 📜 License

This project is created for **educational purposes**.
