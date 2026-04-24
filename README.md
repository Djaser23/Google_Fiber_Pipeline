# Google Fiber Callback Analysis: ETL Pipeline & BI Dashboard

## Overview
This project analyzes repeat customer support calls across three Google Fiber 
markets (New York, Chicago, San Francisco) to identify which issue types and 
markets generate the highest callback rates, and how those rates trend over time.

The goal: help customer service leadership understand where first-contact 
resolution is failing and where to prioritize operational improvements.

## Key Finding
New York account management has a callback ratio of 2.156 — more than double 
any other market/issue combination. New York scheduling and San Francisco 
scheduling are the next highest priorities at 0.767 and 0.544 respectively. 
Chicago shows consistently low callback ratios across all issue types.

## What I Built
**ETL Pipeline (Python/pandas):** Extracts raw contact data, detects and 
corrects illogical callback records (31 identified), imputes missing values, 
engineers a total_callbacks feature, and outputs a clean CSV for Tableau.

**BI Dashboard (Tableau):** Five views covering average callback ratio by 
market and issue type, weekly trend lines by market, weekday volume patterns, 
and a filterable callback ratio table by week. Filters support year, quarter, 
month, and week-level analysis.

## Tech Stack
- Python, pandas
- Tableau Public

## Dashboard
[View on Tableau Public](https://public.tableau.com/app/profile/douglas.jaser/viz/GoogleFiberDashboard_17473459544510/TotalCallbacksbyDateMarket)
