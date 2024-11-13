
# Index Creation and Performance with Large Datasets

This task will help you understand the importance of indexing in handling large datasets by observing query performance on a table with a large number of rows.

## Task: Index Creation and Analysis on Large Datasets

**Objective**: Create indexes on specific columns in a sample database, and measure query performance before and after indexing on large datasets.

### Instructions

1. **Set Up the Table and Populate Data**:
   - Create an `Accounts` table with columns for `customer_id`, `name`, `city`, and `join_date`.
   - Populate the table with a large dataset (e.g., 1 million rows or more). You can use loops, bulk insert scripts, or data generation tools to achieve this.

   ```sql
   CREATE TABLE Accounts (
       customer_id INT PRIMARY KEY,
       name VARCHAR(100),
       city VARCHAR(50),
       join_date DATE
   );
   
   -- Sample code to insert rows - adapt this for larger datasets
   INSERT INTO Accounts (customer_id, name, city, join_date)
   VALUES (1, 'Alice', 'New York', '2023-01-15'), 
          (2, 'Bob', 'Los Angeles', '2023-02-20'),
          (3, 'Charlie', 'Chicago', '2023-03-10');
   ```

2. **Measure Initial Query Performance**:
   - Run a query to select records from the `Accounts` table based on the `city` column.
   - Measure and record the execution time without an index on `city`.

   ```sql
   SELECT * FROM Accounts WHERE city = 'Chicago';
   ```

3. **Create an Index**:
   - Create an index on the `city` column to improve query performance.

   ```sql
   CREATE INDEX idx_city ON Accounts(city);
   ```

4. **Re-run the Query and Measure Performance**:
   - Run the same query again and measure the execution time with the new index on `city`.
   - Record and compare the times before and after indexing.

5. **Scale the Data (Optional)**:
   - If possible, scale up to 10 million or 100 million rows, then re-run the indexed and non-indexed queries to observe performance at a larger scale.

6. **Use `EXPLAIN` to Analyze**:
   - Before and after indexing, use `EXPLAIN` to analyze how the query is executed.
   
   ```sql
   EXPLAIN SELECT * FROM Accounts WHERE city = 'Chicago';
   ```

**Questions for Reflection**:
- How did the execution time change after creating the index?
- What did `EXPLAIN` reveal about the query’s execution plan before and after indexing?
- How does the index impact performance as the dataset grows to millions of rows?
