# Task: Querying Data Using Relational Algebra 

## Description
In this task, you will write and solve relational algebra queries to manipulate and retrieve data from a given set of tables. The goal is to familiarize yourself with the core operations of relational algebra, such as selection, projection, union, and joins.

## Objective
Understand how to apply relational algebra operations to extract and manipulate data from a relational database. Practice translating real-world queries into relational algebra expressions.

## Scenario: University Database
You are provided with the following tables from a university database:

- **STUDENTS** (`StudentID`, `FirstName`, `LastName`, `Major`)
- **COURSES** (`CourseID`, `CourseName`, `Credits`)
- **ENROLLMENTS** (`StudentID`, `CourseID`, `Grade`)

Using these tables, write relational algebra queries to answer the following questions:

---

## Part 1: 

1. **Selection**: Retrieve all students who are majoring in "Computer Science".
   - *Hint*: Use the selection operation (σ).

2. **Projection**: Display only the first and last names of all students.
   - *Hint*: Use the projection operation (π).

---

## Part 2: 

3. **Join**: Find the names of all students enrolled in the "Database Systems" course.
   - *Hint*: Use a natural join (⨝) between the `ENROLLMENTS` and `COURSES` tables.

4. **Set Operations**: Retrieve the list of students who are enrolled in courses but have not received a grade yet.
   - *Hint*: Use set difference (-).

---

## Part 3: 

5. **Set Difference**: Retrieve the list of students who are not enrolled in any courses.
   - *Hint*: Use set difference between the `STUDENTS` and `ENROLLMENTS` tables to find students without any enrollment records.

6. **Cross Product**: Generate a list of all possible student and course combinations (whether enrolled or not).
   - *Hint*: Use cross product between the `STUDENTS` and `COURSES` tables to create all combinations of students and courses.

7. **Selection and Join**: Find the names of students who are enrolled in any course with 3 or more credits.
   - *Hint*: Perform a join between `STUDENTS`, `ENROLLMENTS`, and `COURSES`, followed by a selection based on the number of credits.

8. **Projection and Set Operations**: Retrieve the first and last names of students who are enrolled in at least one course and compare it with students who have not enrolled in any course.
   - *Hint*: Use projection to retrieve student names from both the `STUDENTS` table and the set of students who are enrolled, then use set difference to find students who have not enrolled.

9. **Join with Set Difference**: Find the students who are enrolled in at least one course but have not yet received any grades.
   - *Hint*: Use a join between `ENROLLMENTS` and `STUDENTS`, and then apply set difference to filter out students who have grades.

10. **Selection with Multiple Conditions**: Find all students majoring in Mathematics who are enrolled in courses that carry 4 or more credits.
    - *Hint*: Use join between `STUDENTS` and `ENROLLMENTS` and then apply selection with multiple conditions (Major and Credits).

---

## Part 4: Creative Challenges

11. **Find Common Enrollments**: Retrieve the list of students who are enrolled in both the "Database Systems" course and the "Calculus" course.
    - *Hint*: Use intersection (∩) between two sets of students enrolled in each course.

12. **Course Enrollment Check**: List students who are enrolled in every course that has "Systems" in its name.
    - *Hint*: Use selection on `COURSES` to find courses with "Systems" in the name, and then perform division to check for students enrolled in all these courses.

