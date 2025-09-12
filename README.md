# Telecom Churn SQL Project

- [Overview](#overview)
- [Data_Description](#Data_Description)
- [Key_Insights](#Key_Insights)
- [Business_Suggestions](#Business_Suggestions)
- [Data_Limitations](#DataLimitations)
- [Technical_SQL_Details](#Technical_SQL_Details)


# Overview

Investigating which customers are churning based on demographics, services, billing, and churn data.

# Data_Description

Telecom churn data set. It has 21 columns and 7044 rows. It's from Kaggle and didn't need cleaning.
I would have removed duplicates, split columns, used =name(Proper) to standardize the headers.
It contains demographics, products, and billing. This data set really should be 3 tables joined on customer ID.

# Key_Insights
Keep in mind the telecom industry's average churn rate is 20-30%.

Customer categories that churn the most. The overall churn rate for all customer categories was 27%

Top Churn

- Seniors              42%
- Electronic check     45%
- No Dependents        33%
- Fiber                42%
- No partner           33%
- Month to month       43%
- < 6 months service   55%

## PowerBI Dashboard Showing Key Categories

<img width="1300" height="733" alt="Telecom_Churn_BarChart" src="https://github.com/user-attachments/assets/ab5b1d8a-68d3-4c27-b249-e5ff56c7a851" />

- Seniors tend to be lower income.
- Singles and those without dependents move more often.
- Fiber customers noticeably churned more. The data set did not break down the cost of service, just the monthly total.

- Spending rate did not lead to churn. In many cases those that spent more kept services for 1-2 years.
- Customers paying by electronic check did churn the most of all payment types.

# Business_Suggestions

- Suggest creating an incentive program for month to month subscribers
- Try to steer customers away from electronic check payments.
- The dataset is limited, but I'd investigate more about fiber optic customers.

# Data_Limitations

The data set did not have dates, therefore a chart with churn rate trends wasn't created. The dataset only had length of account called tenure.

# Technical_SQL_Details


Used MYSQL for exploratory data analysis.  Churn is the rate of which customers cancel all services. Focused on using COUNTS and GROUP BY to see which categories of cusotmers had the highest churn rate. 

[Telecom SQL Queries.docx](https://github.com/user-attachments/files/17779596/Telecom.SQL.Queries.docx)




