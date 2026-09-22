# Task 14 — Subscription Plan Mix by Country

## Business Question

How does the subscription plan mix differ across countries?

## Analysis

The analysis compares the number and share of customers across subscription plans in each country.

Customer counts were calculated for each Country × Plan combination using `QUERY` and `SUMIFS`. The share of each subscription plan within a country was then calculated as the number of customers on the plan divided by the total number of classified customers in that country.

A 100% stacked column chart was used to visualize the subscription plan mix across countries.

## Key Finding

The chart shows that the Residential plan is the most popular subscription plan in every country, accounting for at least 57% of customers. The Mini plan has the smallest customer share across all countries.

## Data Quality Note

One customer in the RawData table has no matching subscription record. This customer is therefore excluded from subscription-level plan analysis.
