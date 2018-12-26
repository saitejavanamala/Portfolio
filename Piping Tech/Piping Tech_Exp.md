### About 
Piping Technology and Products is a pipe supports manufacturing company based in Houston, Texas.  I am working with Piping Tech as a Project Engineer. 

### Activities
* Increased Daily Average Production by 46% (1500 lbs to 2200 lbs) through exploratory data analysis using Advanced Excel (Pivot tables, VBA Macros, Power query, Data modeling, VLOOKUP, HLOOKUP) and R programming (dplyr, ggplot2, tidyr, readr).

## We have become consistent.
### ![We are Improving](https://github.com/saitejavanamala/Portfolio/blob/master/Piping%20Tech/WeAreImproving.png)

* Decreased Average Material Identification Time metric by aprox. 60% (11 minutes to 4.5 minutes) by utilizing MS SQL Server for writing SQL queries leading to 20% increase in Daily Average Production metric. 

![Results](https://github.com/saitejavanamala/Portfolio/blob/master/Piping%20Tech/MatIdTime.png)


```sql
---Created a multi-valued subquery

SELECT Job + '-' + Item AS PossibleMatch 
FROM Jobs.CompleteList 
WHERE PartCategory = "TS 2x2x1/4x24" A 500 GR. B" AND PartComments = "%holes" AND FinalFinish = "PAINT 2"
AND Job  IN (SELECT Job + '-' + Item FROM Jobs.CompleteList 
	    WHERE PartCategory = "W 6 x 15 x 78" AND 
	    PartComments IS NULL AND FinalFinish = "PAINT 2");
	    
```

* Generated summary statistics and production reports using Tableau and R (tidyr, ggplot2).


* Implemented Lean Six Sigma techniques (fish-bone diagram, pareto analysis, 5S, 5 WHYS) and utilized Companion by Minitab to create graphs and forms.

#### ![A sample fishbone diagram to pinpoint major issues and to come up with solutions](https://github.com/saitejavanamala/Portfolio/blob/master/Piping%20Tech/Fishbone.PNG)

* Created project presentations using Microsoft PowerPoint and Microsoft Visio for proposals and meetings


* Documented Standard Operating Procedures for Assembly and Shipping operations using Business Process Modeling Notation (BPMN).


* Utilized company's Enterprise Resource Management (ERP) system, Bill of Materials (BOM), AutoCAD drawings, for data mining and decision-making. 

