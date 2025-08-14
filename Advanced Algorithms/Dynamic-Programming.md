## Task 1: Implement Edit Distance for Typo Correction

**Problem Statement:**  
Given a misspelled word and a correct word, compute the minimum number of operations to convert one to the other.  
Allowed operations: insert, delete, or replace a character.

**Input Example:**
misspelled = "kitten"
correct = "sitting"


**Expected Output:**
3


**Objective:**  
- Implement a **DP-based solution** to calculate the minimum number of edits.  
- Explore **tabulation** or **memoization** techniques.  
- Use this edit distance metric to compare against multiple words in a dictionary later.

**Hint:**  
Use a 2D DP table where `dp[i][j]` represents the cost of converting the first `i` letters of `misspelled` to the first `j` letters of `correct`.

**Constraints:**
- Strings contain only lowercase letters.
- Length ≤ 100.


## Task 2: Reconstruct the Optimal Edit Path

**Problem Statement:**  
After computing the minimum edit distance between a misspelled word and a correct word using dynamic programming, implement a method to **backtrack through the DP table** and reconstruct the sequence of operations (insert, delete, replace) that transform the misspelled word into the correct one.

**Input Example:**
misspelled = "kitten"
correct = "sitting"


**Expected Output:**

Operations:

Replace 'k' with 's'
Replace 'e' with 'i'
Insert 'g' at the end


**Objective:**  
- Traverse the filled DP table **backwards** to trace the exact operations used.  
- Understand how each choice (insert, delete, replace, match) leads to the optimal result.  
- Return both the number of steps and the step-by-step transformation path.

**Optional Extension:**  
Given a list of valid dictionary words, use the edit distance approach to find the **closest match** to a given misspelled word.

**Hint:**  
Start from `dp[m][n]` and walk your way back to `dp[0][0]`, choosing the operation (replace, insert, delete) that led to the current value.

**Constraints:**
- The solution must reflect the **minimum edit path** (not just any valid path).
