# Airline Route Profitability Dashboard

## Project Overview
This Power BI project analyses airline route profitability across short-haul, medium-haul, and long-haul flights in 2024.  
The goal was to evaluate route-level financial performance, identify loss-making routes, and highlight where high load factors do not translate into strong profitability.

## Business Objective
- Assess route profitability across the airline network.
- Compare revenue, cost, profit, and profit margin by route and season.
- Identify underperforming routes and route categories.
- Support better pricing and cost-related decisions.

## Tools Used
- Power BI
- Power Query
- DAX
- CSV dataset

## Dataset
The project uses a flight-level dataset with operational and financial information for airline routes in 2024.  
Key fields include:
- Route
- Destination
- Flight_Hours
- Season
- Load_Factor
- Total_Revenue
- Total_Cost
- Profit
- Profit_Margin

## Data Preparation
The main preparation steps included:
- Importing and validating the CSV dataset.
- Checking data types and business logic.
- Creating DAX measures for revenue, cost, profit, and margin.
- Building a clean route category field for reporting.
- Designing an interactive dashboard with slicers and KPIs.

## Data Quality Improvement
A new field, `Route_Category_Clean`, was added because the original `Route_Category` used inconsistent category ranges.  
The new field was created using `Flight_Hours` with clear non-overlapping rules:
- Short Haul: < 3 hours
- Middle Haul: 3 to < 6 hours
- Long Haul: >= 6 hours

## Key Measures
- Total Revenue
- Total Cost
- Total Profit
- Profit Margin %
- Load Factor %
- Loss-Making Flights %
- Route Profitability by Category

## Dashboard Structure
The dashboard includes:
- KPI cards for Revenue, Profit, Profit Margin, and Load Factor
- Route profitability table with conditional formatting
- Monthly revenue and profit margin trend
- Visual breakdown by route category
- Slicers for Season and Route Category

## Key Insights
- 2024: **~$575M** route revenue, **24% profit margin**, but **~35% of flights are loss-making**, so better **ticket pricing and cost management** are needed.
- **Long-haul is weak:** average margin is **~16%**, with **SFO and LAX** at only **~3%** even in peak season.
- **Medium-haul is the profit engine:** **FRA and SIN** deliver margins **above 45%**, while **LHR** is loss-making for most of the year and only slightly profitable in peak season.
- **Short-haul risk:** **~35% of short-haul flights are unprofitable** despite load factors above **70%**.

## Business Impact
This dashboard helps identify which routes are profitable and which are unprofitable.  
It also shows that strong seat occupancy alone is not enough: route profitability depends on both pricing and cost structure.

## Files in This Repository
- `README.md` — project documentation
- `airline_route_profitability.pbix` — Power BI dashboard file
- `airline_route_profitability.csv` — source dataset
- `images/` — dashboard screenshots

## About Me
I am a Junior Commercial Analyst with a strong interest in data analytics, finance, and Power BI.  
This project is part of my analytics portfolio and reflects my focus on turning business data into clear, practical insights.
