# SQL: Concepts & Projects

## Concepts
In SQL, I have been coding using many concepts:
1. I can perform sorting using Order BY, filtering using WHERE clause and predicates such as AND, OR, IN, BETWEEN, LIKE, NOT, Wildcards etc.
2. I have used all kinds of JOINS: LEFT JOIN, RIGHT JOIN, INNER JOIN, CROSS JOIN and set operators such as UNION, UNION ALL, INTERSECT, EXCEPT.
4. I have written both scalar and multivalued subqueries. 
5. With respect to functions: I know Aggregate functions, Window functions, Date and Time, Mathematical, Logical functions, Conversion functions. Also, functions dealing with null values such as ISNULL, NULLIF, COALESCE. 
6. I can use GROUP BY, GROUPING SETS, PIVOT, UNPIVOT for calculating subtotals and grand totals.

" [*Show the complete list.*](https://github.com/saitejavanamala/Portfolio/blob/master/SQL/SQLConceptsInDetail.md)


## Projects

### Piping Technology & Products

```sql
---Create a multi-valued subquery

SELECT Job + '-' + Item AS PossibleMatch 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2";
AND Job  IN (SELECT Job + '-' + Item FROM Jobs.CompleteList 
	    WHERE PartCategory = "W 6 x 15 x 78" AND 
	    PartComments IS NULL AND FinalFinish = "PAINT 2";
	    
```

```sql
---The same result could be achieved with INTERSECT

SELECT Job + '-' + Item AS PossibleMatch 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2" ;

INTERSECT

SELECT Job + '-' + Item  
FROM Jobs.CompleteList 
WHERE PartCategory = "W 6 x 15 x 78" AND 
PartComments IS NULL AND FinalFinish = "PAINT 2";
      
```

### AdventureWorksLT



