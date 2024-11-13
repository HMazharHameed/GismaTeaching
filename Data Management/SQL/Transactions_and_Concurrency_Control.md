
# Hands-on Labs: Transactions and Concurrency Control

These tasks are designed to help you practice and solidify your understanding of transactions and concurrency control in SQL. 

| Task | Further Information |
|------|-------------------------------|
| **1. Implementing a Simple Transaction**: Create a transaction that simulates a bank transfer. Write SQL statements to debit an amount from one account and credit it to another. Use `BEGIN`, `COMMIT`, and `ROLLBACK` to manage the transaction in case of an error. 
| **2. Exploring ACID Properties**: Write queries to demonstrate each of the ACID properties. For example, simulate Atomicity by intentionally causing an error in a multi-step transaction to observe the rollback. 
| **3. Using Isolation Levels**: Set up two concurrent transactions to see the effects of different isolation levels. Demonstrate phenomena like dirty reads, non-repeatable reads, and phantom reads.
| **4. Handling Concurrency with Locks**: Write SQL statements to create a table and implement row-level locking. Practice scenarios where two users try to update the same row simultaneously to see how locks prevent conflicts. 
| **5. Research Task - Concurrency Control Methods**: Read about the different types of locks (e.g., shared vs. exclusive) and their role in concurrency control. Summarize what you learned and how it applies to database design. 

