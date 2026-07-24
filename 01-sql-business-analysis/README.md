# SQL Business Analysis — Northwind Database

End-to-end SQL project answering 20 real business questions on a relational sales database, covering everything from basic filtering to window functions and CTEs.

## 📊 Overview

This project simulates the kind of ad-hoc analysis a Data Analyst is asked to do day-to-day: pull customer/order/product insights from a relational database to answer specific business questions, using nothing but SQL.

**Dataset:** [Northwind](https://github.com/dalers/mywind) (MySQL port) — a classic sample e-commerce database with customers, orders, order details, products, employees, and shippers.

**Tools:** MySQL, MySQL Workbench

## 🎯 Business Questions Answered

The 20 queries progress from foundational to advanced, grouped into four skill areas:

1. **Filtering & Joins** — e.g. orders by a specific customer, products in a category, orders shipped to a specific region
2. **Aggregation (GROUP BY / HAVING)** — e.g. total orders per customer, revenue per product, average order value
3. **Multi-table Joins (3+ tables)** — e.g. full order details combining customer, employee, and shipper info; customers who never ordered
4. **Window Functions & CTEs** — e.g. ranking customers by spend, running totals over time, month-over-month revenue change, top 3 products per category using CTEs

## 🔑 Key Skills Demonstrated

- Multi-table JOINs (INNER, LEFT)
- Aggregate functions with GROUP BY / HAVING
- Subqueries and derived tables
- Window functions: `RANK()`, `ROW_NUMBER()`, `LAG()`, running totals with `SUM() OVER()`
- Common Table Expressions (CTEs), including layered CTEs
- Translating open-ended business questions into precise SQL logic

## 📁 Files

| File | Description |
|---|---|
| `northwind_sql_business_analysis.sql` | All 20 queries with comments |
| `schema/northwind-default-current-timestamp.sql` | Database structure (run first) |
| `schema/northwind-data.sql` | Sample data (run second) |

## ▶️ How to Run This

1. Create a database: `CREATE DATABASE northwind;`
2. Load the structure: run `schema/northwind-default-current-timestamp.sql`
3. Load the data: run `schema/northwind-data.sql`
4. Run any query from `northwind_sql_business_analysis.sql` against the `northwind` database
