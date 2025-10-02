# Task 7: Basic Sales Summary from SQLite Database

## Objective
Use SQL inside Python to pull sales info (total quantity, total revenue), display results, and plot a bar chart.

## Steps
- Created a small SQLite database (`sales_data.db`) with a `sales` table.
- Inserted sample product sales data.
- Ran an SQL query:
  ```sql
  SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue
  FROM sales
  GROUP BY product;
