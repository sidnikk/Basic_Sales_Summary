# Basic_Sales_Summary
# Task 6 - Basic Sales Summary from SQLite Database

## Objective:
To connect Python with an SQLite database, run SQL queries to calculate total quantity sold and revenue, and visualize results using a bar chart.

## Technologies:
- Python
- SQLite3
- pandas
- matplotlib

## Steps Performed:
1. Connected to SQLite database using `sqlite3`.
2. Queried total quantity and revenue per product using SQL.
3. Loaded data into pandas for further processing.
4. Printed the results in the terminal.
5. Created a simple bar chart of revenue by product using matplotlib.

## SQL Used:
```sql
SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
