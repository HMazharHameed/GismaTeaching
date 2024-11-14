
# Task: Banking System with Different Account Types

## Instructions

### Define the `BankAccount` Abstract Class:
1. Add a `balance` field to hold the account balance.
2. Add a constructor to initialize the balance.
3. Create an abstract method `calculateInterest()` that will be implemented by subclasses to calculate interest differently based on account type.
4. Create a concrete method `deposit(double amount)` that adds money to the account balance.
5. Create a concrete method `withdraw(double amount)` that subtracts money from the balance, but only if the balance is sufficient.

### Implement `SavingsAccount`:
- Extend `BankAccount` with a `SavingsAccount` class.
- Override `calculateInterest()` to provide interest based on a fixed interest rate (e.g., 3% of the balance).
- This class should represent a savings account that earns interest.

### Implement `CheckingAccount`:
- Extend `BankAccount` with a `CheckingAccount` class.
- Override `calculateInterest()` to provide no interest (interest rate of 0%).
- This class should represent a basic checking account with no interest.

### Testing in the Main Class:
1. Create instances of `SavingsAccount` and `CheckingAccount`.
2. Test the `deposit`, `withdraw`, and `calculateInterest` methods on each account type.
