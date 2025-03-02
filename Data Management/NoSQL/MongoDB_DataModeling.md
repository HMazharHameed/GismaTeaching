# MongoDB Data Modeling and Aggregation Framework

##  Task 1: Understanding Data Modeling  
Explain in your own words:  
1. The difference between embedding and referencing in MongoDB.  
2. When would you choose embedding over referencing? Provide an example use case.  

---

##  Task 2: Designing a NoSQL Schema  
1. Create a **database** called `ecommerce_db`.  
2. Design a **collection** named `orders` with the following fields:  
   - `order_id`: Unique identifier for the order.  
   - `customer_name`: Name of the customer.  
   - `items`: An array of items (each item should have `product_name`, `price`, and `quantity`).  
   - `total_price`: The total cost of the order.  
   - `order_date`: The timestamp when the order was placed.  
3. Insert three sample orders into the `orders` collection.  

---

## Task 3: Querying Embedded Data  
Write queries to:  
1. Find all orders where the total price is greater than 100.  
2. Retrieve orders that contain a specific product name in the `items` array.  
3. Fetch only the customer_name and `total_price` fields for all orders.  

---

## Task 4: Using the Aggregation Framework 
1. Write an aggregation query to:  
   - Calculate the total revenue (sum of all `total_price`).  
   - Count how many orders were placed per customer.  
   - Find the average order value.  
2. Execute the queries and include both the commands and outputs in your submission.  

---

