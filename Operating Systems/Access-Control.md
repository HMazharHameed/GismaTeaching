## Task 1: Designing a Basic User Authentication and Access Control System

**Scenario:**  
You are designing a small authentication and access control system for a university's online portal.  
The portal must differentiate between two types of users: **Administrators** and **Students**.

**Requirements:**
- Design a simple authentication system where users log in with a username and password.
- After login, the system should check the user's role:
  - **Administrators** can add new courses, view all student records, and modify data.
  - **Students** can view their own records and enroll in courses but cannot modify system settings.

**Objective:**
- Understand how authentication verifies identity.
- Learn how role-based access control restricts what actions users are allowed to perform.

**Hints:**
- Think about simple username/password storage (no need for real encryption).
- Role checking is enough for access control (you don't need full access matrices yet).

**Note:**
Focus on clarity and structure. Advanced security (like hashing passwords) is not required.
