# Starlink Customer & Revenue Analytics

Data analytics portfolio project built with Google Sheets using a simulated Starlink customer dataset.
## Project Overview

This project analyzes a simulated Starlink customer dataset to identify patterns in customer distribution, revenue, subscription plans, discounts, and customer value.

The analysis was performed using Google Sheets, with SQL-style analytical approaches and spreadsheet functions.
## Dataset

The dataset contains 10,001 simulated customers across 10 countries.

The analysis uses two related datasets:

- `starlink_customers.csv` — customer information, including country and customer ID.
- `subscriptions.csv` — subscription plans, monthly fees, discounts, and customer IDs.

The datasets are linked using the customer ID.
## Tools & Skills

- Google Sheets
- SQL-style data analysis
- QUERY
- XLOOKUP
- ARRAYFORMULA
- SUMIF / SUMIFS
- COUNTIF / COUNTIFS
- FILTER
- UNIQUE
- SORT
- Data segmentation
- Data visualization
- Business analysis
## Analysis

The project includes a series of analytical tasks covering different aspects of the customer base and revenue performance:

1. Customer distribution by country
2. Revenue by country
3. Average revenue per customer by country
4. Revenue by subscription plan
5. Discount analysis
6. Customer value by subscription plan
7. Discount effectiveness
8. Customer segmentation by revenue
9. Customer value by country
10. Customer value visualization
11. Customer segment distribution by country
12. Revenue contribution by country
13. Customer signups by month
14. Subscription plan mix by country
15. Revenue share vs customer share by country
## Key Findings

- Customer distribution is relatively even across countries, with a maximum difference of approximately 10%.
- Total revenue and average revenue per customer are also relatively consistent across countries.
- The Residential plan generates the highest total revenue due to its large customer base.
- Business customers generate the highest average revenue per customer.
- Customers without discounts generate higher average revenue per customer than customers receiving large discounts.
- High Value customers represent a smaller share of the customer base but contribute a higher share of total revenue.
- Japan has the highest average revenue per customer and the highest share of High Value customers.
- Customer value distribution is relatively consistent across countries.
## Dashboard

The project includes an interactive Google Sheets dashboard
summarizing key customer and revenue metrics.

The dashboard includes:

- Total customers
- Total revenue
- Average revenue per customer
- High Value customer share
- Revenue by country
- Average revenue per customer by country
- Customer value distribution by country
## Project Structure
```text
starlink-google-sheets-analytics/
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
│   └── task-13-customer-signups-by-month.md
│   └── task-14-subscription-plan-mix-by-country.md
│   └── task-15-revenue-share-vs-customer-share-by-country.md
├── data/
│   ├── starlink_customers.csv
│   └── subscriptions.csv
├── dashboard/
└── google-sheets/
    └── Starlink_Analytics.xlsx
