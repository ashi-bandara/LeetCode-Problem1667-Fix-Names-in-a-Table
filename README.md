
# LeetCode Challenge D12
## Achievements
[![image.png](https://i.postimg.cc/HkYBpNwJ/image.png)](https://postimg.cc/2Vt4G2Xm)

This solution outperformed 63.12% of MySQL users on LeetCode according to runtime metrics and 100% of users according to memory metrics.


## Overview

Welcome to my LeetCode solution repository! This project addresses the coding challenge presented by [1667.  Fix Names in a Table](https://leetcode.com/problems/fix-names-in-a-table/) Below, you'll find details about the problem, my approach to solving it, and the implemented solution.

## Problem Statement
Table:  `Users`

| Column Name |   Type  |
|:-----------:|:-------:|
|   user_id   |   int   |
|     name    | varchar |

user_id is the primary key (column with unique values) for this table.
This table contains the ID and the name of the user. The name consists of only lowercase and uppercase characters.
Write a solution to fix the names so that only the first character is uppercase and the rest are lowercase.

Return the result table ordered by  `user_id`.

The result format is in the following example.


**Example**

> **Input:** 
> Users table:
> 
| user_id | name  |
|:-------:|:-----:|
| 1       | aLice |
| 2       | bOB   |
> **Output:**
> 
>
| user_id | name  |
|:-------:|:-----:|
| 1       | Alice |
| 2       | Bob   |

**Language Used**
> MySQL

**Difficulty**

> Easy



## Solution Overview

- The `UPPER` function is used to convert the first character of each name to uppercase. 

- The `LOWER` function is used to convert the remaining characters of each name to lowercase. 

- The `CONCAT` function combines the uppercase first character with the lowercase rest, resulting in the fixed name format. 

- The query does not include an explicit `ORDER BY` clause to ensure that the result set maintains the original order of users in the `Users` table.
