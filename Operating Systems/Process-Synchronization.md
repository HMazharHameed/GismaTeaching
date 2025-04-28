## Task 1: Accessing and Modifying a Shared Resource

**Description:**  
Create a program where multiple processes or threads attempt to access and modify a shared resource at the same time.  
The shared resource could be a simple counter, a bank account balance, an inventory stock, or a ticket counter.

**Requirements:**  
- Create at least two processes or threads.  
- All processes/threads must attempt to modify the same shared resource without any synchronization mechanism.  
- Let the program run multiple times and observe if the final result is different or incorrect.

**Objective:**  
Learn through practice why access to shared resources must be carefully controlled when multiple execution units are involved.
