# OOP Tasks

## Task 1: Define a Class with Public and Private Access
**Objective**: Create a `Person` class with private attributes and public methods to access them.

- Define a `Person` class with the following private attributes:
  - `name` (String)
  - `age` (int)
- Create public getter and setter methods for these attributes to ensure encapsulation.
- Write a main program to:
  - Create a `Person` object.
  - Set the attributes using the setter methods.
  - Display the attributes using the getter methods.

---

## Task 2: Encapsulation with Constructors
**Objective**: Practice using constructors and encapsulation in Java.

- Add a constructor to the `Person` class that initializes the `name` and `age` attributes.
- Modify the main program to:
  - Create a `Person` object using this constructor.
- Add a method `displayInfo()` that prints out the person’s details.

---

## Task 3: Public vs. Private Methods
**Objective**: Distinguish between public and private methods.

- Add a private method to the `Person` class called `calculateAgeCategory()`. This method should return a string such as "Child", "Adult", or "Senior" based on the person’s age.
- Modify the `displayInfo()` method to call `calculateAgeCategory()` within it, and display the person’s age category along with their details.

---

## Task 4: Inheritance - Extend the Person Class
**Objective**: Introduce inheritance by creating subclasses.

- Create two subclasses, `Student` and `Employee`, that inherit from the `Person` class.
- Add additional attributes:
  - `Student`: `studentID` (String), `major` (String)
  - `Employee`: `employeeID` (String), `position` (String)
- Override the `displayInfo()` method in both subclasses to display the new attributes.
- Write a main program to create both `Student` and `Employee` objects and display their details.

---

## Task 5: Polymorphism - Method Overloading and Overriding
**Objective**: Understand method overloading and method overriding.

- Overload the `displayInfo()` method in the `Person` class to allow it to accept a boolean parameter:
  - If `true`, display detailed information (name, age, and the result of `calculateAgeCategory()`).
  - If `false`, display only the name and age.
- Demonstrate method overriding by calling `displayInfo()` from the `Student` and `Employee` subclasses.

---

## Task 6: Interface Implementation - Comparable Interface
**Objective**: Implement interfaces to compare `Person` objects.

- Make the `Person` class implement the `Comparable<Person>` interface.
- Implement the `compareTo()` method to compare persons based on their age.
- Write a program to:
  - Create a list of `Person` objects with different ages.
  - Sort the list using `Collections.sort()`.
  - Print the sorted list of persons by age.

---