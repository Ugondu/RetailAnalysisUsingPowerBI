# Analysing Factors Contributing to Revenue and Growth Of an E-Commerce Company using PowerBI



![image](https://github.com/user-attachments/assets/39158d1b-b740-498b-9d31-0ede064ceebd)




# Table of Contents
- [Objective](#objective)
- [Data Source](#data-source)
- [Stages](#stages)
- [Design](#design)
  - [Mockup](#mockup)
  - [Tools](#tools)
- [Development](#development)
  - [Data Exploration](#data-exploration)
  - [Data Cleaning](#data-cleaning)
- [Visualization](#visualization)
  - [Results](#results)
  - [DAX Measures](#dax-measures)
- [Analysis](#analysis)
  - [Findings](#findings)
  - [Insights](#insights)
- [Recommendations](#recommendations)



# Objective

- What is the business problem?

An online retail store wants a detailed insights into the major contributors to the revenue and growth to aid in their planning for the next business year.

- What could be the ideal solution?

As a data consultant, creating a visualization on PowerBI from the dataset made available will answer the business problem. The visualisation would include;

- The total revenue over time period
- Quantity of goods sold
- Number of active customers over a time period
- Top ten customers by revenue
- Quantity of goods sold by country
- Top 10 countries by reveune and number of units sold
- Sales trend over time in the year 2011.

This will aid and guide the organisation on the areas to upscale or downscale as the case may be.

## User story

The leadership of the company are intrested in viewing the metrics from both an operations and marketing perspective to determine the major contributors to the revenue of the company. The CEO and COO are keen on expansion, and would require data driven guidance to attain their company goals for the next business year.

# Data Source

- What data will be suitable to answer the business questions?

The dataset should include;
- Invoice number
- Stock code
- Description
- Quantity
- Invoice date
- Unit Price
- Customer ID
- Country

The dataset is made available in an Excel format and can be accessed here, [see here to find it](https://github.com/Ugondu/RetailAnalysisUsingPowerBI/blob/main/Assets/dataset/Online%20Retail%20Data.xlsx)

# Stages

- Design
- Development
- Analysis

# Design

## Dashboard template

To create a detailed and insightful dashboard, understanding the business questions is crucial.

1. What is the overall revenue generated over the time period in the data available?
2. How many units of items were sold over this period?
3. What is the total number of active customers in our database?
4. Who are the top 10 customers by revenue generation?
5. Which countries have the demand for our products?
6. How has revenue trended over the months in 2011?
7. What are the top 10 countries by revenue and units sold?


## Dashboard mockup

- The final template should contain

1. Column chart
2. Map
3. Line chart
4. Score cards
5. Bar charts


![image](https://github.com/user-attachments/assets/63c3b1ae-17ca-432e-bf28-a739128ab96b)

## Tools
| Tool | Purpose |
| --- | --- |
| Excel | Exploring the data |
| Power BI | Visualizing the data via interactive dashboards |
| Mokkup AI | Designing the wireframe/mockup of the dashboard | 
| GitHub | Hosting the project documentation and version control |

# Development

- What is the best approach to create an end to end solution for the client?

1. Get the available data
2. Explore the data using Excel
3. Clean the data using Excel
4. Load data into Power Bi
5. Transform the data using Power BI
6. Visualize the data using Power BI
7. Generate the findings based on insights
8. Present findings to the board.

## Data Exploration

This stage typically involves an overview of the dataset for inconsistencies, whitespaces, errors, corrupted characters, and blank fields.

## Data Cleaning

The aim is to normalise and structure our dataset ready for analysis.

The cleaned data should meet the following requirement:

- The quantities should not be below zero
- The unit price should not be below zero
- Contain columns relevant to the analysis
- All data types should be appropriate for the fields in each column
- No null and blank fields in the dataset indicating complete data for all record.

# Visualization

## Results

The final dashboard shows a detailed analysis based on the pain points of the company leadership board.

![image](https://github.com/user-attachments/assets/a754c0ff-e6d1-46a2-9bb2-9eb318375a8f)

## Dax Measures

### 1. Unit Sold 
```dax
Unit sold (M) = 
VAR SumofUnitSold = SUM(Sales[Quantity])

Return SumofUnitSold
```

### 2. Total Revenue
```dax
Revenue (M) = 
Var TotalSales = SUM(Sales[Total sales])

Return TotalSales
```

### 3. Total Customers

```dax
Customers = COUNTA(Customer_dimension_table[CustomerID])
```

# Analysis

## Findings

#### 1. Who are the top 10 customers by revenue generation?

| Rank | Customer ID            | Total contributions($) |
|------|------------------------|------------------------|
| 1    | 14646                  |   280,000              | 
| 2    | 18102                  |   260,000              |
| 3    | 17450                  |   190,000              |
| 4    | 16446                  |   170,000              |
| 5    | 14911                  |   140,000              |
| 6    | 12415                  |   120,000              | 
| 7    | 14156                  |   120,000              |
| 8    | 17511                  |   90,000               |
| 9    | 12346                  |   80,000               |
| 10   | 16029                  |   70,000               |


#### 2. What are the top 10 countries by revenue and units sold?

| Rank | Country                | Total Revenue($)       |  unit sold(m) |
|------|------------------------|------------------------|---------------|
| 1    | Netherlands            |   280,000              |  200,000      |
| 2    | EIRE                   |   260,000              |  150,000      |
| 3    | Germany                |   200,000              |  120,000      |
| 4    | France                 |   170,000              |  110,000      |
| 5    | Australia              |   140,000              |   80,000      |
| 6    | Spain                  |   55,725               |   27,731      |
| 7    | Switzerland            |   53,087               |   30,527      |
| 8    | Japan                  |   37,416               |   26,000      |
| 9    | Belguim                |   36,927               |   22.962      |
| 10   | Sweden                 |   36,869               |   36,043      |


#### 3. How has revenue trended over the months in 2011?

For better understanding, attached is a visualisation of the trend.


![image](https://github.com/user-attachments/assets/a74a1efb-d9ef-4d9d-9ecd-43ca4d5cbf2b)



# Insights

Our analysis shows that store sales are impacted by seasonality which occurred in the last 4 months of the year.
Increase in revenue started in the month of September with a 40% increase from August, while revenue remained constant in the first 8 months of the year. In the month of November, revenue peaked at $1.5m which is the highest for the year 2011.

Our analysis uncovered that most of the sales are in the European region with a few in the American regions. 
African and Asia have little demand of the product, alongside Russia Federation. 

Excluding the United Kingdom, European countries such as The Netherlands, Ireland, Germany, France, and Australia are generating high revenue for the company. 
Thus, business leaders should look to invest more into these countries to increase demand for products.

We demonstrated the absence of significant differences in the purchasing power of top 10 customers. We are able to show that the business is not relying on a few customers, showing that the business is in good position.

# Recommendations

1. Given the surge in revenue in the last four months of the year, we recommend that the company invest more in these products that appear to be seasonal.
2. The board should look into investing more in the high revenue generating countries like The Netherlands, Germany, France, and Ireland to capture more market shares as the products are in demand in these countries.
3. Targetting new regions such as Africa and Asia should be high on the company's list as demand for products in these regions are very low. New strategies such as discounts should be considered in these regions.


