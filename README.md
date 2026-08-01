<<<<<<< HEAD
# Customers and Products Analysis Using SQL

## About this project

This project analyzes a sample sales database (`stores.db`, SQLite) containing customers, products,
orders, order details, payments, employees, and offices.

The analysis questions are based on a guided project's practice prompts. I solved each query on my
own, and in a few places I modified or extended the original
prompts (e.g. handling edge cases like zero/negative quantities that weren't explicitly asked about).

## Files

- `stores.db` — SQLite database with the source tables
- `Analysis.ipynb` — Jupyter notebook containing all queries and results, run with Python (`sqlite3` +
  `pandas`)

## Analyses included

1. **List of Tables** — lists all tables in the database.
2. **Database Overview** — number of columns and rows for each table.
3. **Priority Products for Restocking** — combines a "low stock" ratio (correlated subquery) with a
   "best sellers" ranking (CTE) to find products that are both running low on stock and selling well.
4. **Profit per Customer** — joins `orders`, `orderdetails`, and `products` to compute total profit
   (`quantityOrdered * (priceEach - buyPrice)`) per customer.
5. **Top 5 VIP Customers** — the 5 most profitable customers, using the profit query as a CTE.
6. **Top 5 Least-Engaged Customers** — the 5 least profitable customers (same CTE, sorted ascending).
7. **Average Customer Profit** — the average profit across all customers, as a baseline for comparison.

## How to run

Open `Analysis.ipynb` in VS Code (or Jupyter/Anaconda) and run the cells in order. Requires Python
with `pandas` and `sqlite3` (built into Python's standard library).
=======
# customers-products-analysis-sql
>>>>>>> 46f0b3982856997eb864e473e38158d6e41219bd
