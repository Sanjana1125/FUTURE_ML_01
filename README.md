# FUTURE_ML_01 - AI Powered Sales Forecasting System

## 🎯 Projecy Overview
This project delivers an end-to-end workflow for monthly retail sales forecasting and dashboarding.
It uses Python (Prophet) for time series modeling and Power BI for interactive visualizations, enabling actionable insights for business decisions.

## Features
- Automated data cleaning and aggregation in Python
- Prophet-based time series forecasting
- Export of forecast and actuals to CSV for BI usage
- Power BI dashboard with:
- Actual vs. forecasted sales trend line
- Monthly and yearly comparison charts

## Data Source: 
-Sample Superstore/retail sales CSV (columns used: Order Date, Sales, [Category/Region/Store, ...])
-After cleaning: aggregated as monthly sales for model building and dashboarding

## Workflow
1. Python Data Preparation
- Load CSV and handle encoding issues
- Clean data, drop duplicates, handle missing values
- Group and aggregate sales by month using pd.resample('ME')
- Export to monthly_actuals.csv

## 2. Prophet Forecasting
- Model sales with Prophet, add holidays
- Generate future monthly forecasts
- Export to monthly_forecast.csv

## 3. Power BI Dashboard
- Import monthly_actuals.csv and monthly_forecast.csv
- Prepare and link tables on date field (Order Date, ds)
- Build visuals:
- Line chart for actual vs. forecast (Order Date as X-axis; Sales and yhat as Y-axis)
- Monthly, yearly bar charts for trend analysis

## How to Run
- Clone this repo and place data files in the root or /data
- Run Python notebook or script for data prep and modeling
- Import generated CSVs into Power BI Desktop
- Follow the dashboard setup instructions or use provided .pbix template

## Example Visuals:
- `Sum of sales by month.jpg`
- `Sum of sales by year.jpg`
- `Sum of sales and sum of yhat by Order Date .jpg`

## Requirements
- Python (pandas, Prophet, cmdstanpy, matplotlib)
- Power BI Desktop
