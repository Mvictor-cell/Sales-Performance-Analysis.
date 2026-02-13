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
<img width="930" height="571" alt="Screenshot 2026-02-12 150303" src="https://github.com/user-attachments/assets/248e5ac8-eb6b-4119-9ee7-ca2c6bfb4aee" />

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
<img width="760" height="121" alt="Screenshot 2026-02-12 142707" src="https://github.com/user-attachments/assets/01a6288a-da3e-4f8f-8d77-1b04984e5504" />

The KPI cards shows the following:  
- Revenue (2018-2022): $35.64bn  
- Total Cost: $41.37M  
- Profit Margin%: 0.36%  
- Total Profit: $12.86bn  
- Total Quantity Sold: 906 units 

Key Insight: This indicates strong growth in both revenue and profitability, showing efficient cost control and improved sales performance year-over-year.

## Top 5 Operators vs Countries
<img width="392" height="237" alt="Screenshot 2026-02-12 144607" src="https://github.com/user-attachments/assets/f07b0b42-4beb-490c-97a3-2abeb19dacda" />

The shows that Tuenti has the highest sales performance In USA compared to other countries while Movistar shows underperfomance accross the top 5 Operators and Countries;
key Insight:  
- USA: High concentration in Tuenti; very little room for competitors.  
- Switzerland: Show most competitive environment for Entel and Claro.  
- United Kingdom: Strong performance for Claro and Bitel behind Tuenti.  
- Venezuela & Uruguay: Very similar profiles, with a healthy split between Tuenti and Entel.

## Total Sales by Brands
<img width="392" height="242" alt="Screenshot 2026-02-12 150930" src="https://github.com/user-attachments/assets/3f8329da-db8c-410f-a6a6-894bc3252499" />

The shows that Lg brand has the highest growth, followed by the apple brand. Making them the key revenue drivers across the years.

- Market Leaders: LG and Apple combined account for 18.3bn in sales, which is more than the other four brands combined (17.4bn).
- There is a substantial drop off (about 41%) in sales volume when moving from the Apple brand to the Huawei & Samsung brands. They both recorded 5.1bn in sales. This shows a highly competitive middle market space.  
- Nokia: Follows with 3.7bn in sales while Motorola rounds out the list at 3.5bn.


## Total Profits by brands
<img width="367" height="242" alt="image" src="https://github.com/user-attachments/assets/310fc37c-88a0-4dee-8085-79183fb16d83" />

The Total Profit charts reveals a fascinating story about efficiency and brand value. While high sales often suggest market dominance, the profit data shows who is actually making the most profits per unit sold.  
The chart shows the total profit made by each brand;
Apple: 5.5M  
Lg: 3.0M  
Hauwei: 1.7M  
Samsung: 1.4M  
Nokia: 1.3M  
Motorola: 1.2M

Key Insights:  
- Apple generated nearly double the profit of its closest competitor (LG), even though it sells less volume. This indicates much higher profit margins and brand positioning.
- LG likely relies on a high volume, lower margin strategy compared to Apple. They move the most product, but convert that revenue into profit at a lower rate.
- Hauwei & Samsung: Even though they have the same market reach (sales), Huawei has a more efficient cost structure Samsung.
- Nokia & Motorola: They both show cosistency in underperformance in both sales and profits

## Percentage of Quantities Sold by Brands
<img width="392" height="240" alt="image" src="https://github.com/user-attachments/assets/9b34a3bf-e855-4cdb-9d86-43704012ed43" />

Key Insights from the Chart  
- Lg holds the top spot with 26.93% of total quantities.  
- Apple follows closely in second place with 24.28%.
- Samsung has a slightly larger share at 14.35%.  
- Huawei trails by a razor-thin margin with 14.24%.

## Monthly Revenue Trend (2018 - 2021)
<img width="392" height="242" alt="image" src="https://github.com/user-attachments/assets/ac3991da-c7d9-4d7c-be57-ce08edaa37a0" />

key Insights: The line Chart shows the following 
- The year 2021 is the highest-performing year by a substantial margin.  
- There is a consistent upward trend starting in September and peaking in December across all four years.  
- Most years experience a slight decline in sales during the May–July period before the late year ramp up begins.
- 2018 vs. 2019: Sales in 2019 started stronger than 2018 and maintained a steady lead throughout the year.


<img width="372" height="221" alt="image" src="https://github.com/user-attachments/assets/f16dbaf6-6f26-4a8f-8e52-0978bdba39d4" />

The table shows a high level view of brand efficiency by comparing total revenue to actual profit, with;
- Hauwei: 61% profit margin, despite selling nearly $4.5bn less than LG, it manages to convert a significantly higher percentage of its revenue into profit.
- Apple: generated the highest total profit at $5.5M with a 38% margin, it effectively balances high sales volume with strong profitability.
- LG: The revenue powerhouse, leading the table with nearly $9.6bn in total sales. However, this scale comes at a cost of efficiency. Its profit margin is 31%, which is below the group total of 36%.
- Samsung & Motorola: The least efficient brands, Samsung 28% and Motorola 29%
Collectively, the brands generated $35.6bn in sales with an average profit margin of 36%.


# Recommendations  
Based on my comprehensive analysis of all the charts provided, here are five, actionable business recommendations:
1.	Prioritize high margin products over high volume ones. Selling less at a higher profit is more sustainable than maintaining massive infrastructure for low margin returns.
2.	Allocate the bulk of your marketing and advertising budget to Q4 to ride the December wave.
3.	Increase focus on high-margin products (like Apple).
4.	Samsung portfolio, focus on cost cutting and supply chain optimization. 
5.	Redirect resources toward the high-performing El Salvador/Colombia corridor.

# Dashboard
<img width="1157" height="631" alt="image" src="https://github.com/user-attachments/assets/7199cbb1-4039-48bd-ae1e-2c27e36aadb4" />

# Conclusion
This dashboard provides a clear and interactive visualization of how business performance evolved from 2018 to 2021. It empowers decision makers to identify profitable countries, track sales growth, and plan future strategies based on data-driven insights.

Connect with Me  
Musa Victor 📧 musavcitor970@gmail.com 💼 Musa Victor









