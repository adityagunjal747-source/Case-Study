
---

# 📊 SQL Case Study Project


---

## 📌 Project Overview

This project is a **SQL Case Study** built to practice and demonstrate:

* **Database schema design** 🏗️
* **Data insertion & management** 📥
* **Business insights through SQL queries** 📈
* **Joins, Aggregations, Subqueries, and Window Functions**

It is designed as a **real-life database problem-solving exercise**, making it useful for:
✔️ SQL learners
✔️ Interview preparation
✔️ Business analytics practice

---

## 🛠️ Features

* ✅ **Database creation scripts** (DDL)
* ✅ **Sample data insertions** (DML)
* ✅ **Case study queries** to solve real-world scenarios
* ✅ Covers **Joins, Group By, Having, Subqueries, and Window Functions**
* ✅ Easy to extend for further analysis

---

## 📂 Project Structure

```bash
📁 SQL-Case-Study
 ┣ 📜 Case Study Project.sql   # Main schema + queries
 ┣ 📜 README.md                # Project documentation
```

---

## 🗄️ Database Schema

The schema includes multiple **interconnected tables** for analysis.
👉 *(You can add an ER diagram here for visual clarity — I recommend generating one in MySQL Workbench and exporting it as PNG to include in GitHub.)*

---

## 📝 Example Queries

🔹 **1. Find the top 5 highest-selling products:**

```sql
SELECT ProductName, SUM(SalesAmount) AS TotalSales
FROM Sales
GROUP BY ProductName
ORDER BY TotalSales DESC
LIMIT 5;
```

🔹 **2. Get monthly revenue trend:**

```sql
SELECT DATE_FORMAT(SaleDate, '%Y-%m') AS Month, SUM(SalesAmount) AS Revenue
FROM Sales
GROUP BY Month
ORDER BY Month;
```

🔹 **3. Find customers with repeat purchases:**

```sql
SELECT CustomerID, COUNT(*) AS Orders
FROM Sales
GROUP BY CustomerID
HAVING COUNT(*) > 1;
```

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/sql-case-study.git
   ```
2. Open **MySQL Workbench / SQL Server / PostgreSQL** (depending on your setup).
3. Run the script `Case Study Project.sql`.
4. Explore queries and modify them for practice.

---

## 🎯 Learning Outcomes

By working through this project, you’ll strengthen:

* SQL **fundamentals** (DDL, DML, Joins, Aggregations)
* **Problem-solving** with real-world data
* **Data analysis & reporting** using SQL
* **Interview readiness** with practical query examples

---



## 📌 Author

👤 **\[Your Name]**
🔗 [GitHub](#) | [LinkedIn](#)

---

