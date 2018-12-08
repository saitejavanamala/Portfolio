### List of Datasets I worked on in SQL:
1. AdventureworksLT2014
2. Piping Technology & Products (Multi-valued subquery)

### Some queries I've written:

```sql
---Create a multi-valued subquery

SELECT Job + '-' + Item AS Possible Match 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2";
AND Job  = (SELECT JOb FROM Jobs.CompleteList 
	    WHERE PartCategory = "W 6 x 15 x 78" AND 
	    PartComments IS NULL AND FinalFinish = "PAINT 2");
	    
```

```sql
---The same result could be achieved with INTERSECT

SELECT Job + '-' + Item AS Possible Match 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2" 

INTERSECT

SELECT Job + '-' + Item  
FROM Jobs.CompleteList 
WHERE PartCategory = "W 6 x 15 x 78" AND 
PartComments IS NULL AND FinalFinish = "PAINT 2");
      
```

### Concepts I am familiar with:
1. Relational Databases
2. Schemas and Object Names
3. SQL Statement Types
4. The SELECT Statement (order of execution by engine, Aliases)
5. Data types (Knowledge of different data types, Implicit and Explicit Conversions: CAST, CONVERT, STR)
6. NULLS (IS NULL, ISNULL, NULLIF, COALESCE, Two variants of CASE Statements)
7. Removing Duplicates using DISTINCT
8. Sorting (ORDER BY, TOP with ORDER BY)
9. Paging through OFFSET and FETCH with ORDER BY clause.
10. Filtering and using Predicates ( =<>, <>, IN, LIKE, BETWEEN, AND, OR, NOT)
11. Defining JOINs (at FROM clause and WHERE clause)
12. Cartesian JOIN
13. INNER JOIN (with JOIN clause using AND for multiple filtering)
14. OUTER JOINS: LEFT, RIGHT and FULL
15. CROSS JOIN (Employee position example)
16. SELF JOIN (Employee - Manager example)
17. UNION ALL & UNION, INTERSECT, EXCEPT (Definitions, Guidelines, Differences, Examples, Knowing which row comes from which table)
18. Built-in Functions:
  a. Scalar Functions (Points, as expressions in queries, deterministic & non-deterministic)
  b. Logical Functions
  c. Window Functions
  d. Aggregate Functions
19. Subqueries 
  a. Scalar subquery, Multi-valued subquery
  b. Self-contained subquery, Corelated subquery

### Places I learnt SQL from:
1. Microsoft: DAT201x Querying Data with Transact-SQL (edx.com)
2. Querying with Transact-SQL (datacamp.com)
3. Fundamentals of SQL (Sololearn)
