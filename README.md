# Student Management System using MySQL

A database management project developed using **MySQL** to store, retrieve, and analyze student information through SQL queries.

## 📌 Project Overview

The Student Management System is a beginner-level DBMS project that demonstrates how student records can be organized and managed using a relational database. It allows users to store student details, retrieve records, filter students based on marks, sort results, and calculate department-wise student counts.

## 🎯 Objectives

- Create and manage a student database.
- Store student details in a structured table.
- Retrieve and filter student records using SQL.
- Analyze student data using aggregate functions.
- Practice fundamental database management concepts.

## 🛠️ Technologies Used

- **Database:** MySQL
- **Language:** SQL
- **Database Tool:** MySQL Workbench

## 🗂️ Database Structure

**Database Name:** `student_management_system`

### Table: `students`

| Column | Data Type | Description |
|---|---|---|
| `student_id` | INT | Unique student identifier and primary key |
| `first_name` | VARCHAR(50) | Student's first name |
| `last_name` | VARCHAR(50) | Student's last name |
| `email` | VARCHAR(100) | Unique email address |
| `department` | VARCHAR(50) | Student's department |
| `marks` | DECIMAL(5,2) | Student's marks |

## ✨ Key Features

- Create a database and student table.
- Insert sample student records.
- Display all student information.
- Filter students based on their marks.
- Calculate department-wise student counts.
- Sort student records by marks in descending order.
- Enforce data integrity using primary key, unique, and not-null constraints.

## 💡 SQL Concepts Demonstrated

- Database and table creation
- Primary keys and auto-increment
- Unique and not-null constraints
- Data insertion using `INSERT INTO`
- Data retrieval using `SELECT`
- Conditional filtering using `WHERE`
- Sorting using `ORDER BY`
- Grouping using `GROUP BY`
- Aggregate functions using `COUNT()`

## ▶️ How to Run the Project

1. Install MySQL Server and MySQL Workbench.
2. Open MySQL Workbench and connect to your MySQL server.
3. Open the `student_management_system.sql` file.
4. Execute the SQL script to create the database, table, and sample records.
5. Run the SELECT queries to view and analyze the data.

**Note:** The script inserts sample records. If the records have already been inserted, execute the `INSERT` statement only when needed to avoid duplicate entries.

## 🧪 Example Queries

### 1. Retrieve all students

```sql
SELECT * FROM students;
```

### 2. Find students scoring more than 70 marks

```sql
SELECT *
FROM students
WHERE marks > 70;
```

### 3. Count students by department

```sql
SELECT department, COUNT(*) AS total_students
FROM students
GROUP BY department;
```

### 4. Sort students by marks

```sql
SELECT *
FROM students
ORDER BY marks DESC;
```

## 📁 Project Files

- `student_management_system.sql` — SQL script containing database creation, table creation, sample data, and queries.
- `README.md` — Project documentation and execution instructions.

## 🚀 Learning Outcomes

- Gained practical experience with MySQL and SQL queries.
- Understood relational table structure and basic data integrity constraints.
- Practiced filtering, sorting, grouping, and aggregate operations.
- Learned to document and publish a database project on GitHub.

## 👨‍💻 Author

**Vemuri Prasanth**

