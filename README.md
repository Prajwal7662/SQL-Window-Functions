Window Functions in SQL
📌 Introduction

Window functions in SQL are special functions that perform calculations across a group of rows related to the current row, while still retaining the individual row details. Unlike aggregate functions that return a single value for a group, window functions return a value for each row in the result set.

⚡ Key Characteristics

They operate on a set of rows called a window.

They do not collapse rows like GROUP BY.

They are always used with the OVER() clause.

They are commonly applied for ranking, calculating running totals, moving averages, and comparisons between rows.

🔑 Types of Window Functions
1. Row Number Functions

Functions like ROW_NUMBER, RANK, and DENSE_RANK are used to assign sequential numbers or ranks to rows, often within partitions of data.

2. Distribution Functions

NTILE is used to distribute rows into a defined number of groups or buckets, such as quartiles or percentiles.

3. Value Functions

Functions like LEAD and LAG help access data from the next or previous row without requiring a self-join.

4. Aggregate Window Functions

Functions such as SUM, AVG, MIN, and MAX can also be used as window functions, allowing calculations like running totals, moving averages, and departmental statistics without grouping the data.

🎯 Use Cases

Assigning ranks to employees based on salary within each department.

Splitting data into percentiles or quartiles for analysis.

Calculating cumulative totals, moving averages, or running sums.

Comparing the current row value with the previous or next row value.

✅ Advantages

Provide more detailed insights compared to aggregate functions.

Avoid complex self-joins and subqueries.

Preserve individual rows while still enabling advanced calculations.

Useful for business analytics, reporting, and trend analysis.

📖 References

SQL Window Functions in standard documentation.

PostgreSQL, SQL Server, MySQL, and Oracle official resources.
