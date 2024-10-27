
# Library Management System

## Overview
In this project, you will design and implement a basic **Library Management System** using Java's Object-Oriented Programming (OOP) principles. 
The system will manage books, members, and the borrowing/returning of books. 
This project combines multiple OOP concepts to create a real-world, interactive example.

## Objective
- Understand and apply basic OOP principles, such as classes, objects, encapsulation, and methods.
- Practice using constructors, getters, setters, and composition to model relationships between classes.
- Implement a small project with real-world relevance, showcasing the interactions between different objects.

## Project Structure
To create the Library Management System, follow the class structures outlined below. 


### 1. Class: `Book`
**Purpose**: Represents a book in the library.

**Given Structure**:
- **Fields**: `title`, `author`, and `isBorrowed`.
- **Constructor**: Initializes title and author, with `isBorrowed` set to `false` by default.

**Your Task**:
- Add public **getters** for `title`, `author`, and `isBorrowed`.
- Implement `borrow` and `returnBook` methods to manage the borrowing status.

### 2. Class: `Member`
**Purpose**: Represents a library member.

**Given Structure**:
- **Fields**: `name`, `memberId`, and a list to track borrowed books.

**Your Task**:
- Implement public **getters** for `name` and `memberId`.
- Create a method to **borrow a book** (adding it to the member’s borrowed books list).
- Create a method to **return a book** (removing it from the borrowed books list).

### 3. Class: `Library`
**Purpose**: Manages books and members in the library.

**Given Structure**:
- **Fields**: Lists to store all `Book` and `Member` objects.

**Methods Provided**:
- **registerMember**: Registers a new library member.
- **addBook**: Adds a book to the library's collection.

**Your Task**:
- **borrowBook**: Find a book by title, mark it as borrowed, and add it to the member’s list.
- **returnBook**: Find a book by title, mark it as returned, and remove it from the member’s list.
- **displayStatus**: Display each book’s status (available or borrowed) and borrower details if applicable.

### 4. Class: `LibraryTest` (Main Program)
**Purpose**: Simulate library operations by adding books, registering members, borrowing/returning books, and displaying library status.


## Suggested Approach
1. **Step-by-Step Implementation**:
   - Start by creating each class with the given fields and methods.
   - Gradually implement methods for each class to ensure correct functionality.
2. **Testing**:
   - Use `LibraryTest` to call each method and verify functionality. Print outputs at each step to validate expected behavior.
3. **Encapsulation and Validation**:
   - Make fields `private` and use getters/setters for access.
   - Validate data, like ensuring only available books can be borrowed.

## Final Output
By the end, your Library Management System should:
- Allow books to be borrowed and returned by members.
- Display the current status of each book in the library.
- Track which member has borrowed each book, showing real-world class interactions.

---

