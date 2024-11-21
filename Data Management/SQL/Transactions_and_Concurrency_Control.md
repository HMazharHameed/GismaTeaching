
# Transactions and Concurrency Control

This task is based on a real-world scenario to help you practice working with transactions in SQL.

## Bank Transfer with Insufficient Balance Check Task  
Simulate a bank transfer between two accounts in the `Accounts` table. The transaction should debit `account_id = 1` by 100 units and credit `account_id = 2` by 100 units, but only if `account_id = 1` has a balance greater than or equal to 100. Use a transaction with conditional `ROLLBACK` to ensure that if the balance is insufficient, the transfer doesn’t proceed.

## Instructions

1. Begin a transaction.
2. Retrieve the balance for `account_id = 1` and check if it is greater than or equal to 100.
3. If the balance is sufficient:
   - Deduct 100 units from `account_id = 1`.
   - Add 100 units to `account_id = 2`.
   - Commit the transaction.
4. If the balance is insufficient, `ROLLBACK` the transaction to cancel any changes.

