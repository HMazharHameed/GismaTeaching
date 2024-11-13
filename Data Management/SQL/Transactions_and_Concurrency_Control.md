
# Transactions and Concurrency Control

These tasks use real-world scenarios to help you practice transactions and concurrency control in SQL. 

## Bank Transfer with Insufficient Balance Check Task  
Simulate a bank transfer between two accounts in the `Accounts` table. The transaction should debit `account_id = 1` by 100 units and credit `account_id = 2` by 100 units, but only if `account_id = 1` has a balance greater than or equal to 100. Use a transaction with conditional `ROLLBACK` to ensure that if the balance is insufficient, the transfer doesn’t proceed.

**Steps**:
1. Begin a transaction.
2. Retrieve the balance for `account_id = 1` and check if it is greater than or equal to 100.
3. If the balance is sufficient:
   - Deduct 100 units from `account_id = 1`.
   - Add 100 units to `account_id = 2`.
   - Commit the transaction.
4. If the balance is insufficient, `ROLLBACK` the transaction to cancel any changes.

## Bank Transaction Concurrency Control Task

## Scenario
Two customers attempt to withdraw 50 units from the same bank account (`account_id = 1`) at the same time. To prevent inconsistencies, you’ll use transactions and locks to control concurrency and ensure data accuracy.

## Instructions

### Step 1: Set Up the Table
Create an `Accounts` table with a starting balance for `account_id = 1`.

### Step 2: Transaction A - Withdraw 50 Units
This transaction attempts to withdraw 50 units from `account_id = 1`. It uses `FOR UPDATE` to lock the row, preventing other transactions from modifying it concurrently.

### Step 3: Transaction B - Concurrent Withdrawal of 50 Units
At the same time, Transaction B also tries to withdraw 50 units from `account_id = 1`. This transaction will wait if Transaction A has locked the row.

## Observations and Questions

1. **Run both transactions**: Execute Transaction A and Transaction B at the same time and observe the locking behavior.
2. **Modify Isolation Level**: Change the isolation level to `SERIALIZABLE` and re-run the transactions. How does this affect concurrency?
3. **Without `FOR UPDATE`**: Try removing `FOR UPDATE` from both transactions. What impact does this have on data consistency?


