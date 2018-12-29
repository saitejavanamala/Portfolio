```sql
---Create a multi-valued subquery

SELECT Job + '-' + Item AS PossibleMatch 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2"
AND Job  IN (SELECT Job + '-' + Item FROM Jobs.CompleteList 
	    WHERE PartCategory = "W 6 x 15 x 78" AND 
	    PartComments IS NULL AND FinalFinish = "PAINT 2");
	    
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
      
