# Task: Designing a Simple Database Using the Relational Model and ERD

## Description
In this exercise, you will learn to identify entities and their attributes for a given scenario, create an Entity-Relationship Diagram (ERD), and then translate it into a relational schema. This task will help you understand how to structure a database using both conceptual (ERD) and logical (relational model) representations.

## Objective
Understand the process of modeling real-world scenarios into database structures using both the relational model and ERD. Learn to identify entities, define attributes, and establish relationships between entities.

## Scenario: Library Management System
Imagine you are tasked with designing a database for a **Library Management System**. The system needs to keep track of the books in the library, the members who borrow books, and the records of borrowed books.

### Part 1: Identify Entities and Attributes
- **Step 1**: Think about the main objects (entities) in a library system that you need to track. Consider what unique identifiers and details (attributes) each entity might have.
  - *Hint*: What are the most important elements to keep track of in a library?
- **Step 2**: For each entity, list the attributes that are necessary to describe it. Focus on attributes that are essential for identifying and managing the entity.
  - *Example*: For a book, you might consider attributes like title, but think about other details too.

### Part 2: Create an ERD
- **Step 1**: Draw an ERD that includes all the entities and their attributes. Use symbols to represent entities (rectangles) and attributes (ovals).
- **Step 2**: Identify the relationships between these entities. How are they connected? Represent these relationships using lines and specify the type of relationship (e.g., one-to-many, many-to-many).
  - *Hint*: Consider how books and members interact within the library system.

### Part 3: Translate ERD to Relational Model
- **Step 1**: Based on your ERD, define the tables you would need in a relational database. Include the primary key for each table and any foreign keys needed to represent relationships.
- **Step 2**: List out the tables with their attributes and keys. Think about how you can use primary and foreign keys to connect your tables logically.

## Questions for Reflection
- Why is it necessary to break down many-to-many relationships using a junction table?
- How does the relational model help in maintaining data integrity and reducing redundancy?