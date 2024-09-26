# Task: Designing a Simple Database Using the Relational Model and ERD

## Description
In this exercise, you will learn to identify entities and their attributes for a given scenario, create an Entity-Relationship Diagram (ERD), and then translate it into a relational schema. This task will help you understand how to structure a database using both conceptual (ERD) and logical (relational model) representations.

## Objective
Understand the process of modeling real-world scenarios into database structures using both the relational model and ERD. Learn to identify entities, define attributes, and establish relationships between entities.

## Scenario: Library Management System
You are tasked with designing a simple database for a **Library Management System**. The system should manage data about books, library members, and the borrowing of books.

### Part 1: Identify Entities and Attributes
- **Entities**:
  - Book
  - Member
  - Loan
- **Attributes**:
  - **Book**: `BookID`, `Title`, `Author`, `ISBN`, `Genre`, `PublicationYear`
  - **Member**: `MemberID`, `FirstName`, `LastName`, `Email`, `PhoneNumber`
  - **Loan**: `LoanID`, `BookID`, `MemberID`, `LoanDate`, `ReturnDate`
- **Primary Keys**:
  - Book: `BookID`
  - Member: `MemberID`
  - Loan: `LoanID`

### Part 2: Create an ERD
- Draw an ERD using appropriate symbols:
  - **Entities**: Use rectangles to represent `Book`, `Member`, and `Loan`.
  - **Attributes**: Use ovals and link them to their corresponding entities.
  - **Relationships**:
    - A `Member` can borrow many `Books`.
    - A `Book` can be borrowed by multiple `Members` over time.
    - Use a connecting line between `Member` and `Book` entities through the `Loan` entity to represent this many-to-many relationship.

### Part 3: Translate ERD to Relational Model
- Define tables based on the ERD:
  - **Books**: `BookID` (PK), `Title`, `Author`, `ISBN`, `Genre`, `PublicationYear`
  - **Members**: `MemberID` (PK), `FirstName`, `LastName`, `Email`, `PhoneNumber`
  - **Loans**: `LoanID` (PK), `BookID` (FK), `MemberID` (FK), `LoanDate`, `ReturnDate`

## Questions for Reflection
- Why is it necessary to break down many-to-many relationships using a junction table (e.g., `Loan`)?
- How does the relational model help in maintaining data integrity and reducing redundancy?

