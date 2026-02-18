## 📊 SQL Data Analysis Project

### 📌 Problem Statement
Analyze employee salary and department data to generate meaningful business insights using SQL queries.

### 🗄️ Database Schema
Table: employees  

| Column      | Type     |
|-------------|----------|
| id          | INT      |
| name        | VARCHAR  |
| department  | VARCHAR  |
| salary      | INT      |

### 💻 SQL Queries Used

```sql
-- Find top 2 highest salaries
SELECT name, salary
FROM employees
ORDER BY salary DESC
LIMIT 2;

-- Department wise average salary
SELECT department, AVG(salary) AS avg_salary
FROM employees
GROUP BY department;

-- Employees earning more than 50000
SELECT name, department, salary
FROM employees
WHERE salary > 50000;


