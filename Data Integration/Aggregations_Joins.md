# Joins and Aggregations in Spark SQL

## Scenario

You are working with a retail analytics team that wants to understand customer purchasing patterns. You have two datasets: one contains customer details, and the other contains order transactions. Your task is to combine and analyze this data using Spark SQL to generate meaningful insights.

---

## Datasets

- `customers.csv`: Contains `customer_id`, `name`, `city`, `signup_date`
- `orders.csv`: Contains `order_id`, `customer_id`, `order_date`, `total_amount`

---

## Task Overview

You will use Spark SQL to perform joins and aggregations to answer business questions such as:
- Which customers placed the most orders?
- What is the average order value per customer?
- Which city generated the highest revenue?

---

## Task Steps

### Step 1: Load the Datasets

- Load both CSV files into Spark DataFrames.
- Print schemas and preview records.

---

### Step 2: Perform Joins

- Perform a join between `customers` and `orders` on `customer_id`.
- Optionally, explore a join to identify customers with no orders.

---

### Step 3: Aggregation Queries

- Calculate the total number of orders per customer.
- Compute the average `total_amount` per customer.
- Group by `city` and compute total revenue generated per city.

---

### Step 4: Insights

- Find the **top 5 customers** by total spend.
- Find the **month** with the highest number of orders (extract month from `order_date`).
- Identify cities with fewer than 3 active customers.


