# Sales Performance Analysis

## Project Overview
An analyzes of order-level sales data using Microsoft Excel and Power Query. The goal is to find which categories, regions, and channels drive revenue and profit, and which rows should be reviewed before anyone trusts the numbers.

## Business Objective
1. Determine the total **Revenue** for each **Product Category**.
2. Analyze the **Profit Margin** of each **Product Category** to evaluate cost efficiency.
3. Compare sales performance (**Revenue & Profit**) across different **Regions**.
4. Identify the **Sales Channel** that contributes the most **Completed** sales.
5. Review the **Monthly Sales Performance** to identify the peak and lowest selling months.
6. Document data quality issues and flag the rows that need review before the dashboard is used for decisions.

## Dataset
The dataset contains 725 order-level sales records, including order date, customer, region, channel, order status, product, quantity, revenue, cost, profit, and sales representative. Orders cover January to June 2026, plus one order in August 2026.

It was built with deliberate data quality problems to practice on: inconsistent text, mixed date formats, missing values, duplicate order IDs, and numbers stored as text.

Source: Dataset 1 (Sales Performance), provided in the Excel Bootcamp Batch 1 by Bayaan.

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

## Data Cleaning Summary
| Stage | Rows |
|---|---|
| Raw data | 725 |
| Used for KPIs (Clean) | 620 |
| Flagged for review | 105 |

The 105 flagged rows are 10 Check Revenue, 8 Check Date, 8 Check Quantity, 5 Duplicate Order, and 74 Review Statuus. They stay in the workbook and are only excluded from the KPI calculations. 

## Key Insights
- Electronics brings in the most revenue from clean rows.
- Stationery has the strongest profit margin, even though its revenue is small.
- Makassar is the top region by clean revenue, but high revenue does not guarantee a high margin.
- Retail has the most orders, while Corporate earns the most completed revenue.
- August has only one order, so it is treated as an anomaly rather than a trend.
- 105 rows were flagged for review and kept out of the dashboard numbers.

## Recommendation
- Prioritize Electronics & Furniture: These two categories drive most of the revenue, so stock and marketing focus should stay strong here.
- Leverage Stationery's Margin: Despite its small revenue, Stationery has the highest profit margin, so it is worth testing more promotion relative to its cost.
- Check Regional Margins: Makassar leads  on revenue, but high revenue does not guarantee high profitability, so compare margins before shifting focus to any region.
- Verify the August Data: August has only one order, so it is an anomaly rather than a real decline. Confirm whether that order is correct or the rest of the month is missing.

## Dashboard Preview
<img width="1692" height="1374" alt="Dashboard Preview" src="https://github.com/user-attachments/assets/7bb0e414-d1f5-42cf-9797-384b8e017883" />

## Files
- [`sales-performance-analysiss.xlsx`](sales-performance-analysiss.xlsx): workbook with raw data, cleaned data, PivotTables, dashboard, business questions, and cleaning log.
- [`dashboard-preview.png`](dashboard-preview.png): Dashboard screenshot
- data-cleaning-log.md: what was wrong with the data and what was done about it
- business-insights.md: answers to the business questions, insights, and recommendations

## Summary Metrics
| Metric | Value |
|---|---|
| Clean Revenue | Rp 1,430,336,900 |
| Clean Profit | Rp 423,861,900 |
| Clean Orders | 620 |
| Profit Margin | 29.6% |
| Average Order Value | Rp 2,306,995 |
| Rows Flagged for Review | 105 |

All metrics use Clean rows only. The 105 flagged rows (duplicate order IDs, blank quantity, date, or revenue, and Returned/Cancelled orders) stay in the workbook but are excluded from these numbers.
