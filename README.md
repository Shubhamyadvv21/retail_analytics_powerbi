# retail_analytics_powerbi
Interactive Power BI dashboard analyzing Superstore sales, profit, and performance across regions and categories. 
# Overview
This project presents an interactive Power BI dashboard that analyzes retail sales and profitability performance across regions, product categories, and time using the Sample Superstore dataset.
It demonstrates the complete analytics workflow — from data cleaning and transformation to data modeling, DAX measures, and insightful visualization.
# Objectives
Analyze total sales, profit, and profit margin across categories and regions.

Track monthly and yearly sales performance.

Identify top-performing products and low-profit segments.

Build a dynamic, interactive dashboard for management decision-making.
# Tools & Technologies Used
| Tool | Purpose |
|------|----------|
| Power BI | Data visualization and dashboard creation |
| Power Query | Data cleaning and transformation |
| DAX | Custom KPIs and calculations |
| Excel | Data source and initial exploration |
| GitHub | Project documentation and version control |
# Key Metrics & DAX Measures

|  *Measure Name* |  *DAX Formula* | *Purpose / Description* |
|----------------------|--------------------|-------------------------------|
| *Total Sales* | SUM(Orders[Sales]) | Calculates total revenue generated from all sales transactions. |
| *Total Profit* | SUM(Orders[Profit]) | Calculates total profit earned from all orders. |
| *Profit Margin %* | DIVIDE([Total Profit], [Total Sales]) | Measures profitability percentage based on total sales. |
| *Total Orders* | DISTINCTCOUNT(Orders[Order ID]) | Counts the total number of unique orders placed. |
| *Average Order Value (AOV)* | DIVIDE([Total Sales], [Total Orders]) | Calculates the average revenue generated per order. |
| *Sales YTD* | CALCULATE([Total Sales], DATESYTD('Date'[Date])) | Calculates cumulative Year-To-Date (YTD) sales. |
| *Sales LY* | CALCULATE([Total Sales], DATEADD('Date'[Date], -1, YEAR)) | Calculates total sales from the same period in the previous year. |
| *Sales YoY %* | DIVIDE([Total Sales] - [Sales LY], [Sales LY]) | Calculates the Year-over-Year growth rate in sales. |

# Dashboard Preview
<img width="1920" height="1080" alt="Screenshot 2025-11-04 234811" src="https://github.com/user-attachments/assets/71e4307e-bc7b-45ec-892b-7a80f9ad7826" />
<img width="1920" height="1015" alt="Screenshot 2025-11-04 234405" src="https://github.com/user-attachments/assets/b2d48f3c-6160-4f3f-a9e1-46022a33b275" />

# Key Insights
Technology category contributes the highest sales (101k) and profit margin (~13%).

West region leads in overall profitability.

overall profit stays at(~12%).

Technology have highest YOY SALES growth.
# Dashboard Features
Interactive KPIs (Sales, Profit, Margin %, Orders, AOV).

yearly Sales Trend (Line Chart).

Profit by Category (Bar Chart).

Regional Sales (Map Chart).

Profitability Table by Sub-Category.

Slicers for Year, Region, and Category.

# Data Workflow
1. Imported Superstore CSV data into Power BI.

2. Cleaned & transformed data in Power Query:

   Removed duplicates, corrected data types, dropped Row ID.

   Replaced invalid dates and standardized region/category names.

3. Created DAX measures for KPIs and time intelligence.

4. Built dashboard visuals for key insights.

5. Exported reports and documented the entire process.
