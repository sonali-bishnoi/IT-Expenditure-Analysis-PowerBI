# IT-Expenditure-Analysis-PowerBI
This project presents an interactive Power BI dashboard designed to analyze an organization's IT expenditure. The dashboard compares Actual, Planned, and Forecasted IT spending to identify budget variances and provide actionable insights for better financial decision-making.  


# Business Problem
The organization is experiencing significant differences between its planned, forecasted, and actual IT expenditure.
Management needs a centralized dashboard to:
- Monitor IT spending
- Identify overspending and underspending
- Compare Actual vs Plan vs Forecast
- Analyze expenditure across Business Areas, Countries, IT Areas, and Cost Elements
- Improve future budgeting decisions


# Dashboard Pages

## Executive Summary
This page provides a high-level overview of IT expenditure.
Key Insights : 
- Total Actual Expenditure
- Total Planned Budget
- Total Forecasted Expenditure
- Plan Variance %
- Actual vs Plan by Business Area
- IT Spend by Cost Element Group
- Country-wise IT Expenditure


## Variance Analysis
This page identifies where budget deviations occur.
Key Insights :
- Variance by Business Area
- Top 10 Cost Elements with Highest Variance
- Variance by IT Area
- Detailed Business Area Matrix


## Future Forecast
This page focuses on future IT expenditure trends.
Key Insights :
- Future Monthly IT Expenditure
- Future Spend by Business Area
- Future Spend by IT Area
- Future Country-wise Expenditure

# Dashboard Preview

## Executive Summary

<img width="663" height="374" alt="image" src="https://github.com/user-attachments/assets/a355c089-bed4-4375-9e96-58c4d4a5c5d1" />

## Variance Analysis

<img width="662" height="376" alt="image" src="https://github.com/user-attachments/assets/b69a9cf0-cb52-4a81-a864-2b54d8b7a4f0" />

## Future Forecast

<img width="662" height="374" alt="image" src="https://github.com/user-attachments/assets/01363e4e-dbd4-4504-8bf9-edf21f0cab42" />

# Tools Used
- Microsoft Power BI Desktop
- Power Query
- DAX
- Microsoft Excel

# Dataset Information
The dataset contains historical and future IT expenditure data.
Main columns include:
- Date
- Business Area
- Region
- Country
- IT Area
- IT Sub Area
- Cost Element Name
- Cost Element Group
- Actual
- Plan
- Forecast

# DAX Measures
The dashboard uses the following measures:

Total Actual = SUM(Data[Actual])

Total Plan = SUM(Data[Plan])

Total Forecast = SUM(Data[Forecast])

Plan Variance =
[Total Actual] - [Total Plan]

Forecast Variance =
[Total Actual] - [Total Forecast]

Plan Variance % =
DIVIDE(
    [Plan Variance],
    [Total Plan]
)

# Key Business Insights
- Infrastructure has the highest IT expenditure.
- Labor contributes the largest share of total IT costs.
- The USA accounts for the highest IT spending.
- Several business areas show significant negative variance against the planned budget.
- Future forecasts indicate continued high investment in Infrastructure and Functional IT Areas.


