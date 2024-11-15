# Telecom Churn SQL Project

## Overview

Investigating which customers are churning based on demographics, services, billing, and churn data.

## Data Description

Telecom churn data set. It has 21 columns and 7044 rows. It's from Kaggle and didn't need cleaning.
I would have removed duplicates, split columns, used =name(Proper) to standardize the headers.
It contains demographics, products, and billing. This data set really should be 3 tables joined on customer ID.

## Key Insights
Keep in mind the telecom industry's average churn rate is 20-30%.

Customer categories that churn the most. The overall churn rate for all customer categories was 27%

Top Churn

Seniors          42%
Singles          33%
Month to month   43%
Fiber            42%
Electronic check 45%

Seniors tend to be lower income.
Singles and those without dependents move more often.
Fiber customers noticeably churned more. The data set did not break down the cost of service, just the monthly total.

Spending rate did not lead to churn. In many cases those that spent more kept services for 1-2 years.
Customers paying by electronic check did churn the most of all payment types.

## Data Limitations

The data set did not have dates, therefore a chart with churn rate trends wasn't created. The dataset only had length of account called tenure.

## Technical Details

Used MYSQL for exploratory data analysis.  Churn is the rate of which customers cancel all services. Focused on using COUNTS and GROUP BY to see which categories of cusotmers had the highest churn rate. 

![TelecomChurn1 (1)](https://github.com/user-attachments/assets/c40f9b88-88d7-4d31-ad06-e707588d668d)


