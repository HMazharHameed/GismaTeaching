# NoSQL Indexing and Performance Tuning


##  Objective
This assignment will test your understanding of indexing strategies, query performance optimization.

---

##  Task 1: Understanding Indexing  
Explain in your own words:  
1. What is an index in MongoDB, and how does it improve query performance?  
2. What is the difference between a single-field index and a compound index?  
3. When would you use a text index in MongoDB?  

---

##  Task 2: Creating and Using Indexes  
1. Create a database called `ecommerce_db`.  
2. Design a collection named `products` with the following fields:  
   - `name`: The product name.  
   - `category`: The product category (e.g., "Electronics", "Clothing").  
   - `price`: The price of the product.  
   - `stock`: The number of items in stock.  
   - `description`: A text description of the product.  
3. Insert five sample product documents into the `products` collection.  
4. Create an index on the `category` field.  
5. Create a compound index on `price` and `stock`.  
6. Create a text index on the `description` field.  

---

##  Task 3: Querying with Indexes  
Write queries to:  
1. Retrieve all products where the category is "Electronics" (using the index).  
2. Find the top three most expensive products in stock (using the compound index).  

---

##  Task 4: Query Performance Analysis  
1. Run the same query with and without an index using the `explain("executionStats")` method.  
2. Compare the query execution times and write a short explanation of your findings.  

---