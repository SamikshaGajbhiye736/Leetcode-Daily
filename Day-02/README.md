# 📘 SQL Problem: Customers Not Referred by Customer 2

## 📌 Problem Statement
We are given a table `Customer` with the following schema:

| Column Name | Type    |
|-------------|---------|
| id          | int     |
| name        | varchar |
| referee_id  | int     |

- `id` is the **primary key**.  
- Each row represents a customer, their name, and the `id` of the customer who referred them (if any).  

We need to **find the names of the customers** that are either:
1. Not referred by customer with `id = 2`, or  
2. Not referred by anyone (`referee_id IS NULL`).  

Return the result table in any order.
