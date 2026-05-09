# Airline Route Profitability Dashboard | Power BI

## Project Overview
This project explores airline route-level profitability for 2024 using a synthetic aviation dataset and a Power BI dashboard.  
The dashboard combines commercial metrics (revenue, load factor, route mix) and financial metrics (profit and margin) to support route and pricing decisions.

## Business Objective
- Measure route-level P&L performance (Revenue, Cost, Profit, Profit Margin %).
- Identify profitable vs loss-making routes and flights.
- Understand how load factor and seasonality impact profitability.
- Provide a clear executive view for commercial and finance stakeholders.

## Dataset
The dataset contains one year of flight-level and route-level data for DXB-based routes, including:[file:123]
- Flight date, origin, destination and route.
- Aircraft type and capacity.
- Passengers and Load Factor %.
- Ticket and ancillary revenue.
- Operating cost breakdown (fuel, maintenance, crew, airport fees, etc.).
- Total Revenue, Total Cost, Profit and Profit Margin %.

> Note: The data is synthetic and created for learning and portfolio purposes only.[file:123]

## Tools and Techniques
- Power BI
- Power Query for data cleaning and transformations
- DAX for calculated measures and KPIs
- Data modelling and dashboard design

## Data Preparation
Key steps:
- Loaded the CSV dataset into Power BI and validated data types.[file:123]
- Built measures for:
  - Total Revenue
  - Total Cost
  - Total Profit
  - Profit Margin % = Profit / Total Revenue
  - Avg Revenue per Pax
  - Avg Load Factor %
  - Route Revenue % (share of total revenue by route)
- Aggregated flight-level data to route-level metrics for the main table.[file:123]
- Created calculated columns for load factor buckets (Low, Medium, High) and seasonality (months / seasons).

## Dashboard Layout

### Executive KPIs
Top KPI cards show:
- Avg Revenue per Pax
- Avg Load Factor %
- Total Flights
- Unique Routes
- Total Route Revenue
- Total Route Profit
- Overall Profit Margin %

These give a quick at-a-glance view of network performance.

### Route Profitability (P&L Summary)
A detailed table presents:
- Route
- Total Revenue
- Total Profit
- Profit Margin %
- Route Revenue %
- Load Factor %

Conditional formatting highlights the most profitable and loss-making routes using a red–green colour scale.

### Flights by Profitability
A pie chart shows the split between profitable and loss-making flights (by count of flights), helping to understand the overall quality of the route network.[file:142][file:123]

### Profit and Revenue by Load Factor
A chart groups flights into load factor buckets (Low <70%, Medium 70–85%, High ≥85%) and compares Total Revenue and Total Profit.  
This reveals how utilisation (LF) is linked to profitability.

### Top 10 Routes by Profit
A bar chart ranks the most profitable routes by Total Profit, highlighting key contributors to the airline’s financial performance.

### Monthly Revenue and Profit Margin
A combo chart shows:
- Total Revenue by month (columns)
- Profit Margin % by month (line)

This exposes seasonality patterns and months with weaker profitability.

## Key Insights
Examples of insights that this dashboard supports:[file:142][file:123]
- A relatively small number of routes generate a significant share of Total Profit and Revenue.
- Some long-haul routes deliver high revenue but low or negative Profit due to high operating costs.
- Flights with Low Load Factor are frequently loss-making, while High LF flights tend to be consistently profitable.
- Certain months show both lower revenue and negative or very low Profit Margin %, suggesting strong seasonality and opportunities for capacity or pricing adjustments.

## Business Value
For airline commercial and finance teams this type of dashboard can:
- Provide a single view of network profitability at route level.
- Prioritise routes for actions (grow, fix, reduce or exit).
- Support discussions between Commercial, Network Planning and Finance using shared KPIs.
- Encourage data-driven decisions around pricing, scheduling and capacity planning.

## Files in this Repository
- `airline_route_profitability.pbix` – Power BI report file.
- `data/airline_route_profitability.csv` – source dataset.
- `images/aviation_route_profitability_2024.png` – main dashboard screenshot.
- `images/route_profitability_table.png` – detailed P&L summary screenshot (optional).
- `README.md` – this project documentation.

## About Me
I am a Junior Commercial and Data Analyst based in Scotland with a background in aviation and travel.  
I am interested in combining data analytics, finance and BI tools to support better commercial decisions. This dashboard is part of my Power BI portfolio.
