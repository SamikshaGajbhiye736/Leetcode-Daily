# SQL Problem – Find Authors Who Viewed Their Own Articles

## Problem Statement  
We are given a table **Views** with the following structure:

| Column Name | Type |
|-------------|------|
| article_id  | int  |
| author_id   | int  |
| viewer_id   | int  |
| view_date   | date |

- Each row indicates that a `viewer_id` viewed an article written by `author_id` on a given date.  
- If `author_id = viewer_id`, it means the author has viewed **their own article**.  
- The task is to **find all authors who viewed at least one of their own articles**.  
- The result must be sorted by `id` in ascending order.  

---

## Example  

### Input:  
```text
+------------+-----------+-----------+------------+
| article_id | author_id | viewer_id | view_date  |
+------------+-----------+-----------+------------+
| 1          | 3         | 5         | 2019-08-01 |
| 1          | 3         | 6         | 2019-08-02 |
| 2          | 7         | 7         | 2019-08-01 |
| 2          | 7         | 6         | 2019-08-02 |
| 4          | 7         | 1         | 2019-07-22 |
| 3          | 4         | 4         | 2019-07-21 |
| 3          | 4         | 4         | 2019-07-21 |
+------------+-----------+-----------+------------+
