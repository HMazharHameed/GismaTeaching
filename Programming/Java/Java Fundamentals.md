
# Java Practice Tasks

## (1) Sum of Two Integers

## Problem Statement

Given two integers `num1` and `num2`, return the sum of the two integers.

## Example 1:
**Input**: num1 = 12, num2 = 5  
**Output**: 17  
**Explanation**: num1 is 12, num2 is 5, and their sum is 12 + 5 = 17, so 17 is returned.

## Example 2:
**Input**: num1 = -10, num2 = 4  
**Output**: -6  
**Explanation**: num1 is -10, num2 is 4, and their sum is -10 + 4 = -6, so -6 is returned.



## (2) Reverse a String

## Problem Statement

Write a function that reverses a string. The input string is given as an array of characters `s`.  

## Example 1:
**Input**:  
`s = ["h","e","l","l","o"]`  
**Output**:  
`["o","l","l","e","h"]`  

## Example 2:
**Input**:  
`s = ["H","a","n","n","a","h"]`  
**Output**:  
`["h","a","n","n","a","H"]` 

## (3) FizzBuzz

## Problem Statement

Given an integer `n`, return a string array `answer` (1-indexed) where:

- `answer[i] == "FizzBuzz"` if `i` is divisible by 3 and 5.
- `answer[i] == "Fizz"` if `i` is divisible by 3.
- `answer[i] == "Buzz"` if `i` is divisible by 5.
- `answer[i] == i` (as a string) if none of the above conditions are true.

## Example 1:
**Input**:  
`n = 3`  
**Output**:  
`["1","2","Fizz"]`

## Example 2:
**Input**:  
`n = 5`  
**Output**:  
`["1","2","Fizz","4","Buzz"]`

## Example 3:
**Input**:  
`n = 15`  
**Output**:  
`["1","2","Fizz","4","Buzz","Fizz","7","8","Fizz","Buzz","11","Fizz","13","14","FizzBuzz"]`



## (4) Two Sum

## Problem Statement

Given an array of integers `nums` and an integer `target`, return the indices of the two numbers such that they add up to `target`.

- You may assume that each input would have exactly one solution, and you may not use the same element twice.
- You can return the answer in any order.

## Example 1:
**Input**:  
`nums = [2,7,11,15]`, `target = 9`  
**Output**:  
`[0, 1]`  
**Explanation**:  
Because `nums[0] + nums[1] == 9`, we return `[0, 1]`.

## Example 2:
**Input**:  
`nums = [3,2,4]`, `target = 6`  
**Output**:  
`[1, 2]`

## Example 3:
**Input**:  
`nums = [3,3]`, `target = 6`  
**Output**:  
`[0, 1]`


## (5) Contains Duplicate

## Problem Statement

Given an integer array `nums`, return `true` if any value appears at least twice in the array, and return `false` if every element is distinct.

## Example 1:
**Input**:  
`nums = [1,2,3,1]`  
**Output**:  
`true`  
**Explanation**:  
The element `1` occurs at the indices 0 and 3.

## Example 2:
**Input**:  
`nums = [1,2,3,4]`  
**Output**:  
`false`  
**Explanation**:  
All elements are distinct.

## Example 3:
**Input**:  
`nums = [1,1,1,3,3,4,3,2,4,2]`  
**Output**:  
`true`


## (6) Count Elements

## Problem Statement

Given an integer array `arr`, count how many elements `x` there are, such that `x + 1` is also in `arr`. If there are duplicates in `arr`, count them separately.

## Example 1:
**Input**:  
`arr = [1,2,3]`  
**Output**:  
`2`  
**Explanation**:  
1 and 2 are counted because 2 and 3 are in `arr`.

## Example 2:
**Input**:  
`arr = [1,1,3,3,5,5,7,7]`  
**Output**:  
`0`  
**Explanation**:  
No numbers are counted because there is no 2, 4, 6, or 8 in `arr`.
