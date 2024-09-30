# Task: Querying Data Using Relational Algebra

## Description
In this task, you will write and solve relational algebra queries to manipulate and retrieve data from a given set of tables. The goal is to familiarize yourself with the core operations of relational algebra, such as selection, projection, union, and joins.

## Objective
Understand how to apply relational algebra operations to extract and manipulate data from a relational database. Practice translating real-world queries into relational algebra expressions.

## Scenario: University Database
You are provided with the following tables from a **University Database**:

- **Students** (`StudentID`, `FirstName`, `LastName`, `Major`)
- **Courses** (`CourseID`, `CourseName`, `Credits`)
- **Enrollments** (`StudentID`, `CourseID`, `Grade`)

Using these tables, write relational algebra queries to answer the following questions:

---

### Part 1: Basic Queries
1. **Selection**: Retrieve all students who are majoring in "Computer Science".
   - *Hint*: Use the selection operation (σ).
   - Example: `σ Major = 'Computer Science' (Students)`

2. **Projection**: Display only the first and last names of all students.
   - *Hint*: Use the projection operation (π).
   - Example: `π FirstName, LastName (Students)`

---

### Part 2: Intermediate Queries
3. **Join**: Find the names of all students enrolled in the "Database Systems" course.
   - *Hint*: Use a natural join (⨝) between the `Enrollments` and `Courses` tables.
   - Example: `π FirstName, LastName (Students ⨝ Enrollments ⨝ σ CourseName = 'Database Systems' (Courses))`

4. **Set Operations**: Retrieve the list of students who are enrolled in courses but have not received a grade yet.
   - *Hint*: Use set difference (-).
   - Example: `(π StudentID (Enrollments)) - (π StudentID (σ Grade IS NOT NULL (Enrollments)))`

---

### Part 3: Advanced Queries
5. **Aggregation**: Find the total number of credits each student is enrolled in.
   - *Hint*: Combine the `Enrollments` and `Courses` tables using a join and perform aggregation.
   - Example: `π StudentID, SUM(Credits) (Enrollments ⨝ Courses)`

