## Task 1: Building a Basic In-Memory File System

**Scenario:**  
You are tasked with building a simplified version of a file system that supports basic operations in memory.  
This will help you understand how real-world file systems manage files and directories internally.

**Requirements:**  
- Create a structure to represent directories and files.
- Implement the following basic operations:
  1. Create a directory
  2. Create a file under a directory
  3. List all contents of a directory
  4. Delete a file
  5. Delete a directory (only if it is empty)

**Expected Behaviors:**
- A directory can contain both files and other directories.
- Paths can be simple strings like `/documents/reports/summary.txt`.
- Assume no duplicate file names inside the same directory.
- Deleting a directory should only succeed if the directory is empty (no files or subfolders).

**Objective:**  
Understand the basics of directory tree structures, file management, and file system operations.

**Hints:**
- Use a tree structure where each node can represent a file or a directory.
- Each directory node can have a list of children (files and subdirectories).
- Each file node is a leaf with a name but no children.

**Note:**  
Focus on correctness and clarity. Optimization (speed or space) is not required.
