# SQL Practice Tasks

Welcome to SQL Practice! This file contains a series of tasks designed to help you develop core SQL skills. Each task provides a detailed description and sample query, covering essential SQL functions. (LeetCode)

---


## Task 1: Retrieve Personal Information with Address

This task involves retrieving personal information along with addresses from two tables: `Person` and `Address`. 
The goal is to list each person's first name, last name, city, and state. If the address information is missing 
for a person, the `city` and `state` should display `NULL`.

## Table Structure

### `Person` Table

| Column Name | Type    |
|-------------|---------|
| personId    | int     |
| lastName    | varchar |
| firstName   | varchar |

- `personId` is the primary key for this table.
- This table contains information about each person's ID, first name, and last name.

### `Address` Table

| Column Name | Type    |
|-------------|---------|
| addressId   | int     |
| personId    | int     |
| city        | varchar |
| state       | varchar |

- `addressId` is the primary key for this table.
- This table contains information about each person's address with city and state.

## Task Description

Write a SQL query to return the first name, last name, city, and state of each person in the `Person` table. 
If there is no corresponding address for a `personId` in the `Address` table, the `city` and `state` values should be `NULL`.

### Example

#### Input

**Person Table:**

| personId | lastName | firstName |
|----------|----------|-----------|
| 1        | Wang     | Allen     |
| 2        | Alice    | Bob       |

**Address Table:**

| addressId | personId | city          | state      |
|-----------|----------|---------------|------------|
| 1         | 2        | New York City | New York   |
| 2         | 3        | Leetcode      | California |

#### Output

| firstName | lastName | city          | state    |
|-----------|----------|---------------|----------|
| Allen     | Wang     | Null          | Null     |
| Bob       | Alice    | New York City | New York |

#### Explanation

- `personId` 1 does not have an address entry, so `city` and `state` are `NULL`.
- `personId` 2 has an address entry in the `Address` table, so `city` and `state` values are returned accordingly.



## Task 2: List All Cities with More Than One Resident

Write a SQL query to find all cities in the `Address` table that have more than one resident. Your query should return only the city names, without duplicates.

## Task 3: List People with More Than One Address

Write a SQL query to find all people who have more than one address recorded in the `Address` table. Display the `firstName` and `lastName` of each person.

## Task 4: Count of People by State

Write a SQL query to count how many people live in each state. The result should display the `state` and the corresponding count of residents in that state. If no one lives in a particular state, that state should not appear in the result.

## Task 5: Find People Living in the Same City

Write a SQL query to list the `firstName` and `lastName` of people who share the same city as at least one other person. The result should not show any duplicate rows for the same city.

## Task 6: Calculate Average Age of People

Write a SQL query to calculate the average age of all people listed in the `Person` table. If there are no people in the table, return `NULL` as the average.


## Task 7: Count People by Initial Letter of Last Name

Write a SQL query that counts how many people have last names starting with each letter.

## Task 8: Calculate the Percentage of Residents per City

Write a SQL query that calculates the percentage of people residing in each city relative to the total number of people in the `Address` table.
