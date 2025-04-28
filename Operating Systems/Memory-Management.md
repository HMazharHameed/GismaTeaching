## Task 1: Designing a Basic Memory Management Structure for Paging

**Scenario:**  
You are developing a basic memory management system for a small device with limited RAM.  
Processes arrive needing memory, and your system must track which pages of each process are stored in which memory frames.

**Requirements:**  
- Design a simple data structure (e.g., a table, array, or list) to store page-to-frame mappings for multiple processes.
- Assume memory is divided into fixed-size **frames** (e.g., 8 frames available).
- Assume each process consists of a few fixed-size **pages** (e.g., Process A has 3 pages, Process B has 4 pages).
- Your data structure must:
  - Store which frame holds which process page.
  - Allow easy lookup to find where a page of a process is stored.
  - Mark frames as free or occupied.

**Objective:**  
Learn how operating systems manage memory using simple data structures to organize page-to-frame mappings.

**Note:**  
No page replacement algorithms are required yet. Focus only on allocation and tracking.
