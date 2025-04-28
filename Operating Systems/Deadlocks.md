## Task 1: Deadlock Scenario – Printing and Scanning System

**Scenario:**  
In a shared office environment, multiple employees need to complete a two-step job:  
1. First, they must access a **Printer**.  
2. Then, they must access a **Scanner**.

However, not all employees request the resources in the same order:
- Some employees request the **Printer first**, then the **Scanner**.
- Others request the **Scanner first**, then the **Printer**.

Because of this inconsistency, a deadlock situation can occur:  
One thread holds the Printer and waits for the Scanner, while another holds the Scanner and waits for the Printer.

**Requirements:**  
- Create at least 4 employee threads.  
- Define two shared resources: **Printer** and **Scanner**.
- Program each thread to request both resources in different orders.
- When you run the program, observe if a deadlock occurs.
- After detecting the deadlock, modify your program to prevent the deadlock (e.g., by using a consistent lock ordering or another strategy you prefer).

**Objective:**  
Understand how deadlocks occur and apply deadlock prevention techniques to ensure safe concurrency.