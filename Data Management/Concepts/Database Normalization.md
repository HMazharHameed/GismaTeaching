# Task: Database Normalization

## Description
In this task, you will apply the principles of database normalization to a sample database schema. The objective is to understand how normalization works and how to apply it to remove redundancy and improve data integrity by progressing through 1NF, 2NF, 3NF, and BCNF.

## Objective
Learn how to apply the first three normal forms (1NF, 2NF, and 3NF) and BCNF to a relational database. By the end of this task, you should be able to recognize unnormalized data and restructure it into a more efficient and reliable format.

---

## Scenario: University Course Registration System
You are provided with a **Course Registration** table that contains the following attributes:

| StudentID | StudentName | CourseID | CourseName | InstructorName | InstructorOffice | CourseTime |
|-----------|-------------|----------|------------|----------------|------------------|------------|
| 001       | John Doe    | CS101    | Database   | Prof. Smith    | Room 202         | 10:00 AM   |
| 001       | John Doe    | CS102    | Algorithms | Prof. Brown    | Room 204         | 11:00 AM   |
| 002       | Jane Smith  | CS101    | Database   | Prof. Smith    | Room 202         | 10:00 AM   |
| 002       | Jane Smith  | CS103    | Networking | Prof. Davis    | Room 205         | 12:00 PM   |

---

### Part 1: Apply First Normal Form (1NF)
- **Step 1**: Identify any **multi-valued attributes** or **repeating groups** in the table.
- **Step 2**: Restructure the table to ensure that it adheres to 1NF by ensuring all attributes have atomic values.

---

### Part 2: Apply Second Normal Form (2NF)
- **Step 1**: Identify if there are any **partial dependencies** in the table, where non-key attributes depend on only part of a composite primary key.
- **Step 2**: Decompose the table into smaller tables to ensure that all non-key attributes depend on the entire primary key.

---

### Part 3: Apply Third Normal Form (3NF)
- **Step 1**: Identify any **transitive dependencies** in the decomposed tables, where non-key attributes depend on other non-key attributes.
- **Step 2**: Remove transitive dependencies by further decomposing the tables, ensuring that all non-key attributes depend only on the primary key.

---

### Part 4: Apply Boyce-Codd Normal Form (BCNF)
- **Step 1**: Check if there are any remaining functional dependencies where a non-primary key column is functionally determining other columns.
- **Step 2**: If such dependencies exist, further decompose the tables to ensure that all determinants are candidate keys.

---

### Submission Instructions
- Provide a new table structure for each step of normalization (1NF, 2NF, 3NF, and BCNF).
- Submit your solutions by listing the decomposed tables for each normal form.
