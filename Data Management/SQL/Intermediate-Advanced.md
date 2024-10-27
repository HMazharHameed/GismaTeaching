
# Advanced SQL Tasks - Stored Procedures and Triggers

This file provides two advanced SQL tasks, one focused on creating stored procedures and another on implementing triggers. 
These tasks are designed to reinforce the concepts of automation and efficient query handling in SQL.

---

## Task 1: Stored Procedure - Combining Tables with Parameters

### Objective

Write a stored procedure that combines data from two tables, `Employees` and `Departments`, based on an optional join type parameter. 
The procedure should accept a parameter to specify the type of join (e.g., INNER, LEFT, RIGHT) and return the combined results accordingly.

### Table Structures

**Employees Table**  
| Column Name | Type    |
|-------------|---------|
| emp_id      | int     |
| emp_name    | varchar |
| dept_id     | int     |

**Departments Table**  
| Column Name | Type    |
|-------------|---------|
| dept_id     | int     |
| dept_name   | varchar |

### Requirements

1. Create a stored procedure named `CombineEmployeeDepartment`.
2. The procedure should accept a parameter `join_type` that specifies the type of join (`INNER`, `LEFT`, or `RIGHT`).
3. Use the specified join type to combine the `Employees` and `Departments` tables on the `dept_id` column.
4. Return the combined results with `emp_id`, `emp_name`, `dept_name`, and any `NULL` values as necessary.


## Task 2: Trigger - Logging Updates to a Table

### Objective

Write a trigger that logs any updates made to the `Salaries` table by recording changes in a separate `Salary_Log` table. The log table should record the employee's ID, the old salary, the new salary, and the timestamp of the change.

### Table Structures

**Salaries Table**  
| Column Name | Type    |
|-------------|---------|
| emp_id      | int     |
| salary      | decimal |

**Salary_Log Table**  
| Column Name   | Type         |
|---------------|--------------|
| log_id        | int (auto-increment) |
| emp_id        | int          |
| old_salary    | decimal      |
| new_salary    | decimal      |
| change_time   | timestamp    |

### Requirements

1. Create a trigger named `LogSalaryUpdate` that activates before an update on the `Salaries` table.
2. The trigger should insert a new record into `Salary_Log` whenever an employee’s salary is updated.
3. The log should include the `emp_id`, `old_salary`, `new_salary`, and the current timestamp as `change_time`.

