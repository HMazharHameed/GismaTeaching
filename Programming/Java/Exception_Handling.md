
# Java Exception Handling Practice Tasks

Here is a list of tasks to deepen your understanding of **exception handling** in Java:

## Task 1: Basic Exception Handling
- **Objective**: Understand the syntax and flow of `try`, `catch`, and `finally` blocks.
- **Task**: Write a program that attempts to divide two numbers provided by the user. Handle `ArithmeticException` for division by zero and print a meaningful message.
- **Challenge**: Add a `finally` block that prints a message indicating that the division operation is complete, regardless of whether an exception occurred.

## Task 2: Handling Multiple Exceptions
- **Objective**: Learn how to handle multiple exception types in a single `try` block.
- **Task**: Create a program that reads a number from a file. Handle `FileNotFoundException` if the file is missing, and `NumberFormatException` if the file contains non-numeric content.
- **Challenge**: Add another `catch` block for a generic `Exception` to handle any unexpected errors.

## Task 3: Custom Exception Creation
- **Objective**: Learn how to create and use custom exceptions.
- **Task**: Define a custom exception called `InvalidAgeException` that is thrown when a user tries to input an age less than 18. Write a method that takes age as input and throws the custom exception if the age is invalid.
- **Challenge**: Modify the program to catch the custom exception and prompt the user to enter a valid age again.

## Task 4: Try-With-Resources for File Handling
- **Objective**: Practice resource management using `try-with-resources`.
- **Task**: Write a program that reads lines from a text file using `BufferedReader` with a `try-with-resources` block.
- **Challenge**: Modify the program to handle any `IOException` that may occur while reading from the file and ensure that the file is closed automatically.

## Task 5: Nested Try-Catch
- **Objective**: Understand how nested `try` blocks work.
- **Task**: Write a program that first attempts to open a file (outer `try` block) and then attempts to parse an integer from each line (inner `try` block). Handle file-related exceptions in the outer `catch` and parsing errors in the inner `catch`.
- **Challenge**: Log different error messages for each level of exception.

## Task 6: Exception Propagation
- **Objective**: Learn how exceptions can propagate through method calls.
- **Task**: Create a method that performs a division operation and throws an exception if the divisor is zero. Call this method from another method and handle the exception there.
- **Challenge**: Modify the program to throw and handle a custom `DivisionByZeroException` in the calling method.

## Task 7: Real-World Simulation
- **Objective**: Apply exception handling to simulate a real-world scenario.
- **Task**: Write a small program that simulates a bank account. Create methods for withdrawing money, which should throw an `InsufficientFundsException` if the withdrawal amount is greater than the balance.
- **Challenge**: Add a `try-catch` block to handle this exception and prompt the user to enter a valid withdrawal amount.

## Task 8: Handling Checked vs. Unchecked Exceptions
- **Objective**: Differentiate between checked and unchecked exceptions.
- **Task**: Write a program that reads from a file and throws a `FileNotFoundException` (checked exception) and a method that divides two integers, which might throw an `ArithmeticException` (unchecked exception).
- **Challenge**: Write a brief explanation of the difference between checked and unchecked exceptions and how they should be handled differently.

## Task 9: Logging Exception Details
- **Objective**: Learn how to log exceptions for debugging.
- **Task**: Use `Logger` or `System.err` to log detailed information about an exception, including its message and stack trace.
- **Challenge**: Create a logging mechanism that writes exceptions to a separate log file for later analysis.

