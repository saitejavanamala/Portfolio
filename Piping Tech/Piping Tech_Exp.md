### About 
Piping Technology and Products is a pipe supports manufacturing company based in Houston, Texas.  I am working with Piping Tech as a Project Engineer. 

### Activities
* Increased Daily Average Production by 46% (1500 lbs to 2200 lbs) through exploratory data analysis using Advanced Excel and R programming (dplyr, ggplot2, tidyr, readr).

## We are trying to be consistent with our metrics!
### ![We are Improving](https://github.com/saitejavanamala/Portfolio/blob/master/Piping%20Tech/WeAreImproving.png)

```R
install.packages("tidyverse")
library(plotly)
library(tidyverse)
PackagesData <- read_delim("C:/Users/Sai Teja/Desktop/R/StrutsReportForR.csv", delim = ',',
                           col_names = c( "NetWeight", "Time"), skip = 1)
glimpse(PackagesData)

Pk1 <- PackagesData %>%
              group_by(Time) %>%
              summarise(TotalWt = sum(NetWeight)) %>%
              arrange(Time)

plot_ly(Pk1, x = ~Time, y = ~TotalWt, type = 'bar') 
```


* Decreased material identification time metric by 70% (15 minutes to 5 minutes) by utilizing MS Access and writing SQL code on MS SQL Server by performing joins, subqueries, intersect, etc. 


* Generated summary statistics and production reports using Tableau and R (tidyr, ggplot2).


* Implemented Lean Six Sigma techniques (fish-bone diagram, pareto analysis, 5S, 5 WHYS) and utilized Companion by Minitab to create graphs and forms.

#### [A sample fishbone diagram to pinpoint major issues and to come up with solutions](https://github.com/saitejavanamala/Portfolio/blob/master/Piping%20Tech/Fishbone.PNG)

* Created project presentations using Microsoft PowerPoint and Microsoft Visio for proposals and meetings


* Documented Standard Operating Procedures for Assembly and Shipping operations using Business Process Modeling Notation (BPMN).


* Utilized company's Enterprise Resource Management (ERP) system, Bill of Materials (BOM), AutoCAD drawings, for data mining and decision-making. 

