# SQL: Concepts & Projects

## Concepts
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum." [*Show the complete list.*](https://github.com/saitejavanamala/Portfolio/blob/master/SQL/SQLConceptsInDetail.md)


## Projects

### Piping Technology & Products

```sql
---Create a multi-valued subquery

SELECT Job + '-' + Item AS Possible Match 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2";
AND Job  IN (SELECT Job + '-' + Item FROM Jobs.CompleteList 
	    WHERE PartCategory = "W 6 x 15 x 78" AND 
	    PartComments IS NULL AND FinalFinish = "PAINT 2";
	    
```

```sql
---The same result could be achieved with INTERSECT

SELECT Job + '-' + Item AS Possible Match 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2" ;

INTERSECT

SELECT Job + '-' + Item  
FROM Jobs.CompleteList 
WHERE PartCategory = "W 6 x 15 x 78" AND 
PartComments IS NULL AND FinalFinish = "PAINT 2";
      
```

### AdventureWorksLT



