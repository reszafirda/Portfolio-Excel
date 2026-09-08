# Sales Performance Analysis

## Project Overview
This project analyzes sales data to understand revenue trends, profit margins, regional performance, and sales channel effectiveness using Microsoft Excel and Power Query.

## Business Objective
1. Determine the total **Revenue** for each **Product Category**.
2. Analyze the **Profit Margin** of each **Product Category** to evaluate cost efficiency.
3. Compare sales performance (**Revenue & Profit**) across different **Regions**.
4. Identify the **Sales Channel** that contributes the highest volume of **Completed** orders.
5. Review the **Monthly Sales Performance** to identify the peak and lowest selling months.

## Dataset
The dataset contains 725 sales order records, including order date, region, category, channel, quantity, revenue, cost, profit, and order status.

## Tools Used
- Microsoft Excel
- Power Query
- Excel formulas
- PivotTable & summary analysis
- Excel PivotChart

## Analysis Process
1. Reviewed the raw dataset and identified data quality issues (missing values, duplicate order IDs, inconsistent text formatting, and raw date formatting).
2. Cleaned the data using Power Query — trimmed whitespace, standardized text casing, and converted data types.
3. Built a rule-based Quality Flag column to categorize each row (Clean, Duplicate Order, Check Quantity, Check Date, Check Revenue, Review Status) without deleting the original raw data.
4. Created PivotTable to summarize revenue and profit by category, region, channel, and month, filtered to validated ("Clean") rows only.
5. Built an interactive dashboard with KPI cards and PivotCharts.
6. Documented business questions and cleaning decisions (see the Business Questions and Cleaning Log Template sheets inside the Excel file).

## Dashboard Preview
<img width="1692" height="1374" alt="Dashboard Preview" src="https://github.com/user-attachments/assets/7bb0e414-d1f5-42cf-9797-384b8e017883" />

## Project Files
- [`sales-performance-analysiss.xlsx`](sales-performance-analysiss.xlsx): Full Excel workbook (Raw Data, Cleaned Data, PivotTables, Business Questions, Cleaning Log, and Dashboard).
- [`dashboard-preview.png`](dashboard-preview.png): Dashboard screenshot

Cleaning decisions and business question answers are documented directly inside the Excel file (Cleaning Log Template and Business Questions sheets), not as separate files.

## Key Insights
- **Total Revenue**: Rp1,430,336,900 generated from 620 validated ("Clean") orders, with 105 rows flagged for review and excluded to protect accuracy.
- **Top Product Category**: Electronics generated the highest revenue (~Rp745,989,000), more than double Furniture in second place.
- **Strongest Profit Margin**: Stationery held the highest profit margin (~46,88%), even though it wasn't the top revenue category — showing stronger cost efficiency.
- **Regional Performance**: Makassar was the top-performing region in both revenue (~Rp327,737,100) and profit (~Rp95,278,100), narrowly ahead of Jakarta. 
- **Sales Channel**: Retail contributed  the most revenue from completed orders, ahead of Corporate, Marketplace, and Online.
- **Monthly Trend**: Revenue peaked in March (~Rp297,174,300) and dropped sharply in August (~Rp495,000), an anomaly worth investigating.

## Recommendation
- **Prioritize Electronics & Furniture**: These two categories drive the majority of revenue — ensure stock and marketing focus stays strong here.
- **Leverage Stationery's Margin**: Despite lower revenue, Stationery's high profit margin makes it worth promoting more aggressively relative to its cost.
- **Investigate the August Drop**: The sharp revenue decline in August should be reviewed — check whether it reflects a real seasonal dip or missing/incomplete data.
- **Replicate Makassar's Successs**: Study what's driving Makassar's strong performance and apply similar strategies to lower-performing regions.
