# Experiment 2.1

**Name:** Aditya Singh

**UID:** 24BCS10266

## Aim

To combine the records of two tables using the `UNION` operator and display the final result.

## Question

Till now, we have joined tables by columns. Now let’s join the data by rows.

We use the concept of **UNION** to do that.

**UNION** helps us to place a table right on top of another table.

There are a set of criteria to be followed while appending the tables:

- The number of columns of the tables should be same.
- The data type of the table should be of the same order of that of the first table.

Below is the query to combine tables `Mfg_Ind` and `Mfg_Int`.

```sql
SELECT *
FROM Mfg_Ind
UNION
SELECT *
FROM Mfg_Int;
```

Below mentioned are the tables `Mfg_Ind` and `Mfg_Int`.

### Table Mfg_Ind

| mfg_id | company |
|--------|----------|
| 1001 | Mahindra |
| 1002 | Tata |

### Table Mfg_Int

| Id | cmp_name |
|----|----------|
| 5 | Hyundai |
| 6 | Suzuki |

After executing the above query we get the below mentioned table.

| mfg_id | company |
|--------|----------|
| 1001 | Mahindra |
| 1002 | Tata |
| 5 | Hyundai |
| 6 | Suzuki |

### Task

Write a query using **UNION** to stack the table `Arts` over `Science` and output the final table.

**Note:**

The `UNION` statement removes the duplicate data in the new table formed.

## SQL Queries Used

```sql
SELECT *
FROM Arts
UNION
SELECT *
FROM Science;
```

## Output

```
Well done, it's correct!
```

## Output Screenshot

![UNION Output](union.png)

## Image Explanation

The screenshot shows the SQL query using the `UNION` operator to combine the records of the `Arts` and `Science` tables. The output panel displays the merged result containing unique rows from both tables, confirming that the query executed successfully.

## Result

The `Arts` and `Science` tables were successfully combined using the `UNION` operator, and the final result displayed all unique records from both tables.
