# Starlink Customer & Revenue Analytics

Customer and revenue analytics portfolio project built with Google Sheets and Power BI.

The project analyzes a simulated Starlink customer and subscription dataset and demonstrates practical data analysis skills, including data cleaning, business analysis, spreadsheet analytics, data modeling, Power Query, and DAX.

---

## Project Overview

The goal of the project is to analyze customer behavior, subscription plans, revenue, discounts, and customer value across different countries.

The analysis follows a typical Data Analyst workflow:

**Business Question → Data → Analysis → Validation → Insight → Conclusion**

The project contains 15 analytical tasks, a Google Sheets dashboard, and an interactive Power BI dashboard.

---

## Dataset

The project uses two related simulated datasets:

- `starlink_customers.csv`
- `subscriptions.csv`

### Dataset characteristics

- 10,001 customers
- 10 countries
- Multiple subscription plans
- Customer revenue data
- Discount information
- Customer status
- Contract/sign-up dates

The two datasets are connected through the customer ID.

---

## Tools & Skills

### Google Sheets

- QUERY
- XLOOKUP
- ARRAYFORMULA
- SUMIF / SUMIFS
- COUNTIF / COUNTIFS
- AVERAGEIF
- FILTER
- UNIQUE
- SORT
- Pivot Tables
- Data validation
- Data visualization
- Dashboard creation

### Power BI

- Power BI Desktop
- Data Modeling
- Relationships
- Power Query
- DAX
- Filter Context
- CALCULATE
- ALL / REMOVEFILTERS
- SUMX / AVERAGEX
- FILTER
- KPI Cards
- Slicers
- Interactive dashboards

### SQL-style Analysis

The analytical approach is also based on SQL concepts such as:

- GROUP BY
- Aggregations
- Filtering
- JOIN logic
- Revenue analysis
- Customer segmentation
- Business-oriented analytical questions

---

# Analysis

The project contains 15 analytical tasks.

1. [Customer Distribution by Country](analysis/task-01-customer-distribution.md)
2. [Revenue by Country](analysis/task-02-revenue-by-country.md)
3. [Average Revenue by Country](analysis/task-03-average-revenue-by-country.md)
4. [Revenue by Subscription Plan](analysis/task-04-revenue-by-subscription-plan.md)
5. [Discount Analysis](analysis/task-05-discount-analysis.md)
6. [Customer Value by Plan](analysis/task-06-customer-value-by-plan.md)
7. [Discount Effectiveness](analysis/task-07-discount-effectiveness.md)
8. [Customer Segmentation](analysis/task-08-customer-segmentation.md)
9. [Country & Customer Value](analysis/task-09-country-customer-value.md)
10. [Customer Value Visualization](analysis/task-10-customer-value-visualization.md)
11. [Customer Segment Distribution](analysis/task-11-customer-segment-distribution.md)
12. [Revenue Contribution by Country](analysis/task-12-revenue-contribution-by-country.md)
13. [Customer Sign-ups by Month](analysis/task-13-customer-signups-by-month.md)
14. [Subscription Plan Mix by Country](analysis/task-14-subscription-plan-mix-by-country.md)
15. [Revenue Share vs Customer Share](analysis/task-15-revenue-share-vs-customer-share-by-country.md)

---

# Key Findings

### Customer Distribution

Customer distribution across countries is relatively balanced, with the difference between countries being approximately 10%.

### Revenue by Country

Spain generates the highest total revenue at approximately **$111.8K**, followed by the United States.

### Subscription Plans

The **Residential** plan generates the highest total revenue due to its large customer base.

The **Business** plan generates the highest average revenue per customer.

| Plan | Customers | Revenue | Avg. Revenue |
|---|---:|---:|---:|
| Residential | 5,959 | $652,512 | $109.50 |
| Business | 1,019 | $232,788 | $228.49 |
| Roam | 2,078 | $151,524 | $72.92 |
| Mini | 944 | $43,110 | $45.67 |

### Discounts

Customers without a discount have the highest average revenue per customer.

- No discount: **$118.91**
- Small discount: **$111.38**
- Large discount: **$100.84**

The available dataset does not contain retention or upgrade history, so the long-term effectiveness of discounts cannot be determined from this analysis alone.

### Customer Segmentation

Customers were divided into three value segments:

- Low Value: < $100
- Medium Value: $100–$199.99
- High Value: ≥ $200

High Value customers represent approximately **10% of the customer base** but contribute approximately **21.5% of total revenue**.

### Country Analysis

Japan has the highest average revenue per customer and the highest share of High Value customers.

At the same time, Spain generates the highest total revenue because of its customer base and revenue per customer.

### Revenue Share vs Customer Share

Revenue share and customer share are closely aligned across countries, with differences generally below one percentage point.

---

# Google Sheets Dashboard

The Google Sheets analysis includes an interactive dashboard with:

- Total Customers
- Total Revenue
- Average Revenue per Customer
- High Value Customer Share
- Revenue by Country
- Average Revenue per Customer by Country
- Customer Value Distribution by Country

The complete workbook is available here:

[Starlink Analytics Workbook](google-sheets/Starlink_Analytics.xlsx)

---

# Power BI Dashboard

The project also includes an interactive Power BI dashboard built using the same customer and subscription datasets.

### Power BI Skills Demonstrated

- Data Modeling
- Relationships
- Power Query
- DAX
- Filter Context
- CALCULATE
- SUMX / AVERAGEX
- FILTER
- Interactive Slicers
- KPI Cards
- Data Visualization

### Dashboard

The final Power BI dashboard includes:

- Total Customers
- Total Revenue
- Average Revenue per Customer
- Active Customer Share
- Revenue by Country
- Revenue by Subscription Plan
- Customer Value Distribution by Country
- Customer Status Distribution

### Global Dashboard Metrics

- **Customers:** 10,001
- **Total Revenue:** $1,079,934
- **Average Revenue per Customer:** $107.98
- **Active Customer Share:** 79.48%

Power BI files:

[Power BI Dashboard](power-bi/Starlink_Analytics.pbix)

[Power BI Documentation](power-bi/README.md)

---

# Data Quality

During the analysis, a data quality issue was identified:

**1 customer record does not have a matching subscription record.**

The unmatched customer was retained in the customer-level dataset but excluded from subscription-level analysis where a subscription record was required.

This demonstrates an important analytical practice: identifying and documenting data quality issues instead of silently removing records.

---

# Project Structure

```text
starlink-google-sheets-analytics/
│
├── analysis/
│   ├── task-01-customer-distribution.md
│   ├── task-02-revenue-by-country.md
│   ├── task-03-average-revenue-by-country.md
│   ├── task-04-revenue-by-subscription-plan.md
│   ├── task-05-discount-analysis.md
│   ├── task-06-customer-value-by-plan.md
│   ├── task-07-discount-effectiveness.md
│   ├── task-08-customer-segmentation.md
│   ├── task-09-country-customer-value.md
│   ├── task-10-customer-value-visualization.md
│   ├── task-11-customer-segment-distribution.md
│   ├── task-12-revenue-contribution-by-country.md
│   ├── task-13-customer-signups-by-month.md
│   ├── task-14-subscription-plan-mix-by-country.md
│   └── task-15-revenue-share-vs-customer-share-by-country.md
│
├── data/
│   ├── starlink_customers.csv
│   └── subscriptions.csv
│
├── dashboard/
│   └── .gitkeep
│
├── google-sheets/
│   ├── .gitkeep
│   └── Starlink_Analytics.xlsx
│
├── power-bi/
│   ├── README.md
│   └── Starlink_Analytics.pbix
│
└── README.md
