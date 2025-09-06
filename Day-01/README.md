# 📦 SQL Problem - Low Fat and Recyclable Products

## 📖 Problem
We are given a table **Products**:

| Column Name | Type  |
|-------------|-------|
| product_id  | int   |
| low_fats    | enum  |
| recyclable  | enum  |

- `product_id` is the **primary key**.  
- `low_fats` ∈ {`'Y'`, `'N'`} → `'Y'` = Low Fat product.  
- `recyclable` ∈ {`'Y'`, `'N'`} → `'Y'` = Recyclable product.  

👉 Task: **Find product IDs that are both low fat and recyclable.**


