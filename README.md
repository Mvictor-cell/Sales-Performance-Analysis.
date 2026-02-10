# SALES PERFORMANCE ANALYSIS USING POWER BI(2018-2022)

# Analysis Overview
This project analyzes phone sales performance across multiple countries, distributors, brands, and operators over time. The goal was to transform raw transactional data into actionable business insights using Power BI, with a strong focus on data modeling, DAX, and time based analysis.
The final dashboard provides stakeholders a robust framework for tracking revenue, profitability, trends, and growth drivers to support better sales and strategic decisions.

# Data Source
The dataset was imported into Power BI and transformed in Power Query.

Sample of the dataset in Excel
<img width="920" height="736" alt="Screenshot 2026-02-09 180806" src="https://github.com/user-attachments/assets/da151b87-c62f-47d2-b37e-cdd8c2962c24" />

<img width="997" height="760" alt="Screenshot 2026-02-09 180854" src="https://github.com/user-attachments/assets/7a9acca2-a120-4241-b52a-4a963b45f95b" />

# Preparation Tools(Data Cleaning & Transformation)
Power Query: Power Query in Power BI was used to extract, clean, shape the data. It was used to develop a pipeline that cut manual processing from 4 hours to 20 minutes

## Key steps performed:

- Total Sales = SUM(Sales[Amount])

- Total Profit = SUM(Sales[Profit])

- Profit Margin = DIVIDE([Profit], [Sales])

- Sales YOY = CALCULATE([Total Saless], SAMEPERIODLASTYEAR(Date_Phones[Date]))

- Sales YTD = TOTALYTD([Total Sales],'Date Phones'[Date])

## Data Model Design

A star schema was implemented for optimal performance and clarity.

- Fact Table: Phone Sales

- Dimension Table: Date Phones

# Data Processing
- Standardized data types for all numeric and date fields

- Removed null values and invalid sales records

- Cleaned text fields using Trim and Clean

- Created calculated columns

- Ensured the Date table contained unique dates

## Skills Demonstrated
- ETL & Data Cleaning: Leveraged Power Query to perform complex data transformations and rigorous cleaning, ensuring data integrity by resolving inconsistencies.

- Advanced Analytics: Developed complex DAX measures to extract deep dive insights and facilitate multilayered performance analysis.

- Strategic Visualization: Engineered intuitive reports and dashboards using purposeful visuals to solve specific business problems and simplify data consumption.

- Diagnostic Thinking: Applied critical analysis to uncover trends, brand disparities, and data uncertainties, translating findings into strategic recommendations.

## Key Analysis Objectives
- Conduct a comprehensive YoY (Year-Over-Year) comparison of Sales, Profit, Cost, and Quantity from 2018 to 2022 to evaluate long-term business health.

- Analyze Yearly revenue fluctuations, growth cycles and historical performance consistency.

- Evaluate sales distribution across the Top 5 Countries— USA, Switzerland, United Kingdom, Venezuela, and Uruguay, to identify high value markets and regional growth drivers.

- Deconstruct sales performance by Brand to isolate market leaders, analyze product-mix efficiency, and identify top performing brands.

- Translate data findings into actionable business insights to support executive decision-making and optimize future sales strategies.


## Insights

Sales Overview














