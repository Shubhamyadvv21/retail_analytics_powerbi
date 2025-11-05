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
Tool	                     Purpose
Power BI Desktop	        Dashboard creation and data modeling
Power BI                  Query	Data cleaning and transformation
DAX                     	Calculations & KPIs
Excel / CSV             	Data source and export
GitHub	                  Version control and portfolio hosting
# Key Metrics & DAX Measures
Measure        	Formula / Description
Total Sales  -	SUM(Orders[Sales])
Total Profit - 	SUM(Orders[Profit])
Profit Margin %-	DIVIDE([Total Profit], [Total Sales])
Total Orders-	DISTINCTCOUNT(Orders[OrderID])https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
Average Order Value (AOV)-	DIVIDE([Total Sales], [Total Orders])
Sales YTD	CALCULATE([Total Sales], DATESYTD('Date'[Date]))
Sales YoY %	-DIVIDE([Total Sales] - [Sales LY], [Sales LY])
# Project Folder Structure
Retail-Analytics/
├─ data_raw/          # Original raw dataset(s)
├─ data_processed/    # Cleaned and transformed data (CSV, notes)
├─ pbix/              # Power BI project file (.pbix)
├─ exports/           # Screenshots, PDFs, presentation files
# Dashboard Preview
Screenshot 2025-11-04 234811.png
Screenshot 2025-11-04 234405.png

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
Profitability Table by Sub-Category
Slicers for Year, Region, and Category
# Data Workflow
1. Imported Superstore CSV data into Power BI.
2. Cleaned & transformed data in Power Query:
Removed duplicates, corrected data types, dropped Row ID.
Replaced invalid dates and standardized region/category names.
3. Created DAX measures for KPIs and time intelligence.
4. Built dashboard visuals for key insights.
5. Exported reports and documented the entire process.
