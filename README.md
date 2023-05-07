## Project Overview

When a customer asks to try on a shoe, the employee goes to the back room and is expected to bring the shoe that the customer wants to try on and an additional 3 pair of shoes to try to sell to them. We are working towards creating an application that will tell the employee what was sold with the requested shoe, focusing on other shoes but also including accessories.

Company Hierarchy (highest to lowest):  
* Division
* Regions
* Districts
* Stores

### My Contribution

I developed a python script to deliver the top 3 shoe and accessory recomendation for every unique shoe that was sold in conjuction with another shoe or accessory. Efforts to improve my knowledge, I am currently working on improving the computational time required to return all the recomendations. A recent improvement of 96% has been achieved at 3 days. I believe there is still room for another 96% improvement at 3 hours.


## DATA PROVIDED  
The Date Range of the data is 11/1/22 to 1/31/23.  
* products.csv – This is the product dimension. Join on DIV and STOCKNO to get the DEPARTMENT.
* store.csv – This is the store dimension. Join on DIV and STORE to get the District, Region and State.
* Departments.txt – A list of shoe/accessory departments
* Store Sales.csv – A list of all products sold by the stores during the date range. This will be the denominator of the 90-95% calculation.
* Nov Sold With.csv, Dec Sold With.csv, Jan Sold With.csv. These are the files that include the Primary Stockno and what Secondary Stocknos were sold with them at the store level. There is not a key on the table.

**Important columns:**
* Div
* Store – join with Div to store.csv to get region, district, state 
* Primary Stockno – Should be joined with the Div to the product dimension to get the department.
* Secondary Stockno - Should be joined with the Div to the product dimension to get the department.
