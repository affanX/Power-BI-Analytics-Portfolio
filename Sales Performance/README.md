# 📊 Sales Performance Dashboard

## 📌 Project Overview
This project analyzes sales performance across regions, product categories, and customer segments using **Power BI**.  
It provides actionable insights for improving profitability, identifying top-performing products, and tracking sales trends over time.


## 🎯 Objectives
- Monitor total sales, profit, and discount impact
- Compare performance across regions and product categories
- Identify high-profit and low-profit products
- Visualize sales trends over time

--------------------------------------------------------------------------------------------------------

##DAX Measures Created
##dax// Core Business Metrics

Total Sales = SUM(Sales[Sales])
Total Profit = SUM(Sales[Profit])
Profit Margin % = DIVIDE([Total Profit], [Total Sales]) * 100

##// Performance Classification
Performance Category = 
IF([Profit Margin %] >= 20, "High Performer",
   IF([Profit Margin %] >= 10, "Medium Performer", 
      "Low Performer"))

-------------------------------------------------------------------------------------------
      
Visualizations Used

Cards: Executive summary KPIs
Line Chart: Time series analysis with date hierarchy
Map: Geographic sales distribution
Table: Performance categorization by country
Area Chart: Cost of Goods Sold vs Sales comparison
Pie Chart: Profit distribution by segment
Slicer: Interactive country filtering

📈 Business Insights

Overall Performance: $92.3M in total sales with 14.10% profit margin
Geographic Distribution: Sales across 5 major markets (US, Canada, Germany, France, Mexico)
Trend Analysis: Clear seasonal patterns visible in monthly data
Performance Segmentation: All countries classified as "Medium Performers" (10-20% margin)

🛠️ Tools & Technologies

Power BI Desktop: Dashboard development and data modeling
DAX: Custom calculations and business logic
Power Query: Data transformation and preparation


