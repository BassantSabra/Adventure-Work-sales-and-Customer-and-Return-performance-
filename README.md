📊 AdventureWorks Sales & Customer Performance Dashboard
1. Project Overview

This Power BI project provides a comprehensive view of sales, customer behavior, and product performance for AdventureWorks. The dashboards help management monitor revenue growth, customer value, returns, and refunds, while identifying areas for optimization through what-if analysis and root cause analysis.

2. Key KPIs

The following KPIs were defined and tracked:

Sales & Profitability

Revenue: $24.9M

Profit: $10.5M

Total Orders: 25.2K

Return Rate: 2.2%

Customer Metrics

Total Customers: 17.4K

Revenue per Customer: $1,431

Top Customer: Maurice Shan → 6 orders, $12.41K revenue

Refund & Returns (Root Cause)

Total Refunds: $21,256

Total Returns: 1,115

Most Refunded Category: Accessories (Tires & Tubes, Helmets, Hydration Packs)

3. Data Preparation (Power Query Steps)

Data was imported from AdventureWorks sales tables and cleaned using Power Query:

Data Cleaning

Removed duplicates, null values, and unused columns.

Standardized date formats.

Created calculated columns for Year, Month, Week.

Transformations

Merged sales, products, and customer tables.

Normalized product categories and subcategories.

Added income level and occupation segmentation for customer analysis.

Modeling

Established star schema (FactSales linked to DimCustomer, DimProduct, DimDate).

Relationships set to single direction for optimized performance.

4. DAX Measures & Calculations

Several measures were created to support analysis:

Revenue = SUM(Sales[SalesAmount])

Profit = SUM(Sales[Profit])

Orders = COUNTROWS(Sales)

Return Rate = (SUM(Returns[Qty]) / SUM(Sales[Qty]))

Revenue per Customer = [Revenue] / DISTINCTCOUNT(Customer[CustomerID])

YoY Growth = (Current Revenue – Previous Year Revenue) / Previous Year Revenue

5. Insights
Revenue & Orders

Revenue shows steady growth with a spike in mid-2021.

Monthly revenue reached $1.83M, up +3.31% from the previous month.

Orders slightly declined (-0.88%), while returns increased (+1.78%).

Customer Performance

Professional customers generated the highest revenue segment.

Top 100 customers contributed $615K in revenue.

Maurice Shan was the top customer with $12.41K revenue.

Product Performance

Bestselling: Mountain Bikes (200 Black, 38 & 42).

Most ordered product type: Tires and Tubes.

Most returned product type: Shorts.

Refund Analysis

Refunds concentrated in Accessories ($21,256).

Within Accessories, Tires and Tubes and Helmets had the largest share.

6. What-If Analysis

Simulated scenarios with price adjustments and discount rates.

Tested impact of reducing return rate by 1% → projected profit increase of ~ $150K annually.

Modeled increased orders per customer (from avg. 1.4 → 2) → potential revenue lift of +20%.

7. Root Cause Analysis (Refunds)

Accessories caused 90%+ of refunds.

Within Accessories:

Tires & Tubes ($7.7K refunds)

Helmets ($4.1K)

Hydration Packs ($1.2K)

Insight: Product quality or supply chain issues in bike accessories are driving refunds.

8. Business Recommendations

Customer Retention: Focus on high-value professional customers with loyalty offers.

Product Improvement: Investigate refund root causes in Tires & Tubes and Helmets.

Order Growth: Encourage cross-selling with bundles to raise orders per customer.

Returns Control: Enhance product descriptions/quality checks to reduce return rate below 2%.

What-If Scenarios: Use discount and return-rate simulations for pricing strategy.

9. Deliverables

Power BI Dashboard (Sales, Customer, Refunds).

Data Model Documentation.

KPI Dictionary (Revenue, Profit, Orders, Return Rate, Refunds, Revenue per Customer).
