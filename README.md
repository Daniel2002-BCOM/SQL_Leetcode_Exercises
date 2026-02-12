# SQL LeetCode Challenges and Learnings

This repository is a curated collection of SQL problems sourced from LeetCode. It serves as a practical guide for mastering SQL concepts through hands-on problem-solving. Each solution is implemented in **MySQL** and includes the full problem context and schema setup.

## 🚀 Overview

The project covers a wide range of SQL techniques, including:
- **Basic Filtering:** `WHERE` clauses, `IN`, and `IS NULL`.
- **String Manipulation:** Advanced pattern matching using `REGEXP`.
- **Aggregations:** Using `GROUP BY`, `SUM`, `COUNT(DISTINCT)`, and `HAVING`.
- **Joins:** Various joins including `LEFT JOIN`, `CROSS JOIN`, and self-joins.
- **Conditional Logic:** `CASE WHEN`, `IF`, and `IFNULL` functions.
- **Date & Time Functions:** Monthly reporting, date intervals (`DATE_ADD`), and `DATEDIFF`.

 Key Challenges Included

| Problem ID | Title | Key Concepts |
| :--- | :--- | :--- |
| 1517 | Find Users With Valid E-Mails | Regular Expressions (Regex) |
| 1757 | Recyclable and Low Fat Products | Simple Filtering |
| 595 | Big Countries | OR conditions, Large Datasets |
| 1565 | Unique Orders and Customers | Monthly Aggregation, `LEFT()` function |
| 1251 | Average Selling Price | Weighted Averages, Joins, `ROUND()` |
| 1280 | Students and Examinations | Cross Joins, Handling Missing Data |
| 1484 | Group Sold Products By The Date | `GROUP_CONCAT` equivalent logic |

## 🛠️ Usage

Each section in the `.sql` file follows a standard format:
1. **Problem Description:** The goal of the query.
2. **Schema:** `CREATE` and `INSERT` statements to set up the local testing environment.
3. **Solution:** The optimized MySQL query.

### Example: Finding Valid Emails
```sql
SELECT * FROM Users
WHERE mail REGEXP '^[A-Za-z][A-Za-z0-9\_\.\-]*@leetcode\.com$';
