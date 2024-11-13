
# Hands-on Labs: Transactions and Concurrency Control

These tasks use real-world scenarios to help you practice transactions and concurrency control in SQL. 

| Task | Link and Further Information |
|------|-------------------------------|
| **1. Bank Transfer Simulation with Error Handling**: You’re working with two tables, `Accounts` and `Transactions`. Write a transaction to simulate a bank transfer from one account to another. Add a deliberate error midway (e.g., dividing by zero or referencing a nonexistent account) to see if the transaction rolls back correctly.|

| **2. Exploring Atomicity and Consistency with Multi-Step Orders**: Consider a table `Orders` for an e-commerce site. Write a transaction to create an order that deducts item quantities from `Inventory`, records the sale in `Sales`, and updates the `Order_History`. |

| **3. Experimenting with Isolation Levels**: Using `BEGIN TRANSACTION`, `COMMIT`, and `ROLLBACK`, set up two concurrent transactions on an `Inventory` table. Use different isolation levels to observe effects like dirty reads or phantom reads. |

| **4. Locking Mechanisms and Row-Level Locks**: Create a table `Bookings` with `room_id` and `reservation_date` columns. Implement row-level locking and attempt to insert conflicting reservations simultaneously. |
