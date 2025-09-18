# Customers Who Visited Without Transactions

## Problem Statement
We have two tables: `Visits` and `Transactions`.  

- `Visits` contains all mall visits by customers.  
- `Transactions` contains all transactions made during those visits.  

**Goal:** Find the customer IDs who visited the mall **without making any transactions** and the **number of such visits** per customer.

---

## Tables

### Visits
| Column Name | Type |
|-------------|------|
| visit_id    | int  |
| customer_id | int  |

- `visit_id` is unique for each visit.

### Transactions
| Column Name    | Type |
|----------------|------|
| transaction_id | int  |
| visit_id       | int  |
| amount         | int  |

- `transaction_id` is unique for each transaction.
    t.transaction_id IS NULL
GR
