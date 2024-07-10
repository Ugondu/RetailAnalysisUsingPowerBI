# Tata Online Retail Customer Analysis.
*![image](https://github.com/Ugondu/TataRetailPowerBiDashboard/assets/113315492/e21ae9b8-be71-4321-afab-d207a4cb1c38)"*
## Table of Contents.
- [Business Overview](#business-overview)
- [Project Objective](#project-objective)
- [Data Sources](#data-sources)
- [Data Processing](#data-processing)
- [Insights and Findings](#insights-and-findings)
- [Conclusion and Recommendation](#conclusion-and-recommendation)
## Business Overview.
An online retail store is interested in understanding the major contributors to the company’s revenue over a period. The business is interested in the metrics from both an operations and marketing perspectives to guide into the areas that perform well so it can focus on what is working.
## Project Objective. 
The aim of the project is to visualise business metrics on a PowerBi dashboard to help influence key business decisions by the business leaders.
To achieve the business objectives.
1.	Examine the dataset for inconsistences, missing values, duplicates, and incorrect data type.
2.	Define metrics such as total sales, overall revenue, and total number of customers on the company database in a particular period.
3.	Explore the data to evaluate the country that generates the highest revenue, and the country that generates the lowest revenue.
4.	Define the top ten revenue generating customers to ensure that they remain satisfied.
5.	Examine the region/country with highest demand for the products.
6.	Provide detailed analysis of revenue generation over the months and years, and why the trends occur.
## Data Sources.
The datasets were made available by Tata group via the link *https://cdn.theforage.com/vinternships/companyassets/ifobHAoMjQs9s6bKS/5XsFFJu2oCLdmYJW2/1654309626143/Online%20Retail%20Data%20Set.xlsx*
### Customer data features:
* Invoice number: Unique identifier given to each invoice assigned to a transaction.
* Stock code: Unique identifier for each product available in stock.
* Description: Each product name.
* Quantity: The number of products each customer purchased.
* Invoice date: The date and time each item was sold to a customer.
* Unit Price: Cost of each product on the catalogue.
* Customer ID: Unique identifier for each customer on the company’s database.
* Country: Geographical location of each customer.
## Data Cleaning.
* Removing negative values: The negative values in “Quantity” and “Unit Price” columns were filtered and removed so no value is less than 1 and $0 respectively.
* Data type conversion: The “Customer ID” and “Stock Code” columns were converted to object data type to enhance our analysis.
* Missing Values: The blank fields were removed from the dataset
* Duplicates: Duplicates values were removed from the dataset
## Insights and Findings.
* Our analysis shows that store sales are impacted by seasonality which occurred in the last 4 months of the year. Increase in revenue started in the month of September with a 40% increase from August, while revenue remained constant in the first 8 months of the year. In the month of November, revenue peaked at $1.5m which is the highest for the year 2011.
* Our analysis uncovered that most of the sales are in the European region with a few in the American regions. African and Asia have little demand of the product, alongside Russia Federation. Excluding the United Kingdom, European countries such as The Netherlands, Ireland, Germany, France, and Australia are generating high revenue for the company. Thus, business leaders should look to invest more into these countries to increase demand for products.
* We demonstrated the absence of significant differences in the purchasing power of top 10 customers. We are able to show that the business is not relying on a few customers, showing that the business is in good position.
## Conclusion and Recommendations
This showcases the effectiveness of business intelligence tools such as PowerBi in providing useful insights in dataset. We are able to demonstrate the importance of metrics in marketing and operations perspectives of a business, and how to effectively channel the company’s expansion campaign strategies. 

