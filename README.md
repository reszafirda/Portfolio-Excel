# Sales Performance Analysis

## Project Overview
This project analyzes sales order data to understand revenue trends, profit margins, regional performance, and sales channel effectiveness using Microsoft Excel and Power Query.

## Business Objective
1. Determine the total **Revenue** for each **Product Category**.
2. Analyze the **Profit Margin** of each **Product Category** to evaluate cost efficiency.
3. Compare sales performance (**Revenue & Profit**) across different **Regions**.
4. Identify the **Sales Channel** that contributes the highest volume of **Completed** orders.
5. Review the **Monthly Sales Performance** to identify the peak and lowest selling months.

## Dataset
725 order records with order date, customer, region, channel, order status, product, quantity, revenue, cost, profit, and sales representative.

It is a practice dataset with planted data quality promblems: mixed text formatting, mixed date formats, missing value, duplicate order IDs, and revenue stored as text.

## Tools Used
- Microsoft Excel
- Power Query
- Excel formulas
- PivotTable and PivotChart
- GitHub documentation

## Analysis Process
1. Reviewed the raw data and the data dictionary.
2. Cleaned the data in Power Query: standardized text, converted dates, and turning text revenue into numbers.
3. Added a Quality Flag column that marks duplicates, blanks, and Returned/Cancelled orders. No row was deleted.
4. Built PivotTable on Clean rows only.
5. Built a dashboard with KPI cards and PivotCharts.
6. Wrote the cleaning log and the business insights.

## Key Insights
- Electronics earns the most revenue.
- Stationery has the best margin and Electronics has the lowest margin.
- Makassar leads on revenue is below Medan and Bandung.
- Retail has the most orders, while Corporate earns the most completed revenue.
- March is the peak month. August has one order only, so it is an anomaly, not a trend.
- 105 of 725 rows were flagged and kept out of the KPIs.

## Dashboard Preview
<img width="1692" height="1374" alt="Dashboard Preview" src="https://github.com/user-attachments/assets/7bb0e414-d1f5-42cf-9797-384b8e017883" />

## Files
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

## Summary Metrics

Metric	Value
Clean Revenue	Rp 1,430,336,900
Clean Profit	Rp 423,861,900
Clean Orders	620
Profit Margin	29.6%
Average Order Value	Rp 2,306,995
Rows Flagged for Review	105

All metrics use Clean rows only. The 105 flagged rows (duplicate order IDs, blank quantity, date, or revenue, and Returned/Cancelled orders) stay in the workbook but are excluded from these numbers.
- **Replicate Makassar's Successs**: Study what's driving Makassar's strong performance and apply similar strategies to lower-performing regions.
