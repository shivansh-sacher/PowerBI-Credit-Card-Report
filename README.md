# Credit Card Report

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Process](#process)
- [Features](#features)
- [Insights](#insights)
- [Learning](#learning)

## Overview

To develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends, enabling stakeholders to monitor and analyze credit card operations effectively.  

![O1](https://github.com/user-attachments/assets/38a4ca01-ea4c-41bf-8b57-37c324b7052b)  


![O2](https://github.com/user-attachments/assets/7f5615b8-4906-45e2-b9ee-8552acd584ad)  


![O3](https://github.com/user-attachments/assets/dece5693-eef7-4c22-9dfa-f19d2c02cf83)  


![O4](https://github.com/user-attachments/assets/de248b0c-c7a6-4c4d-bb39-1f39e5c643b4)  

<img width="852" height="231" alt="calculations" src="https://github.com/user-attachments/assets/04551329-e7b7-4297-8d14-89e80ef8fc65" />  

## Dataset


### Customer Profile Table (`cust_detail`)

This table contains detailed demographic and socioeconomic information for each customer.

| Column                     | Description                                                        |
|----------------------------|--------------------------------------------------------------------|
| **Client_Num**             | Unique identifier for each customer                                |
| **Customer_Age**           | Age of the customer (in years)                                     |
| **Gender**                 | Gender of the customer ("M", "F")                                  |
| **Dependent_Count**        | Number of dependents supported by the customer                     |
| **Education_Level**        | Highest level of education attained                                |
| **Marital_Status**         | Marital status ("Single", "Married", etc.)                         |
| **State_cd**               | State code representing the state of residence                     |
| **Zipcode**                | Residential zip/postal code                                        |
| **Car_Owner**              | Indicates if the customer owns a car ("yes"/"no")                  |
| **House_Owner**            | Indicates if the customer owns a house ("yes"/"no")                |
| **Personal_Loan**          | Indicates if customer has a personal loan ("yes"/"no")             |
| **Contact**                | Preferred method of contact (e.g., cellular, telephone, etc.)      |
| **Customer_Job**           | Principal occupation or profession                                 |
| **Income**                 | Customer's reported income (typically annual)                      |
| **Cust_Satisfaction_Score**| Satisfaction score for the customer (higher value = more satisfied)|

### Credit Card Transaction Table (`cc_detail`)

This table captures credit card account details and transactional data for each customer.

| Column                    | Description                                                        |
|---------------------------|--------------------------------------------------------------------|
| **Client_Num**            | Unique identifier for each customer (links to customer profile)    |
| **Card_Category**         | Credit card category/type (e.g., Blue)                             |
| **Annual_Fees**           | Annual fee charged for the credit card                             |
| **Activation_30_Days**    | Was the Card activation in 30 days ("0"/"1")                       |
| **Customer_Acq_Cost**     | Cost to acquire the customer (marketing, onboarding)               |
| **Week_Start_Date**       | Date marking the start of the reporting week                       |
| **Week_Num**              | Week number or label in the year                                   |
| **Qtr**                   | Financial quarter ("Q1", "Q2", etc.)                               |
| **current_year**          | Reporting year                                                     |
| **Credit_Limit**          | Credit limit assigned to customer's card                           |
| **Total_Revolving_Bal**   | Revolving balance not paid in full                                 |
| **Total_Trans_Amt**       | Total amount spent in transactions for the period                  |
| **Total_Trans_Ct**        | Number of transactions in the period                               |
| **Avg_Utilization_Ratio** | Credit utilization ratio (used/available limit)                    |
| **Use_Chip**              | Indicates if card chip is used ("Chip", "Swipe")                   |
| **Exp_Type**              | Most common type of customer expenditure (e.g., Travel, Bills)     |
| **Interest_Earned**       | Interest generated from the account                                |
| **Delinquent_Acc**        | Delinquent account ("0" = no delinquency or "1" = Delinquent)      |



## Process

Tools Used :- Microsoft Excel, PostgresSQL, Microsoft Power BI.  

Process:-   
-Familiarizing with the dataset.  
-Uploading the dataset from CSV file to PostgresSQL.    
-Connecting the data to a Power BI file.    
-Performing Data Cleaning Operations.  
-Generating required Column for analysis.  
-Checking Data Module.     
-Generating Calculations where required.  
-Designing a Power BI dashboard.  
-Creating data visuals for the Power BI dashboard as per the design.  
-Formatting the Visuals.  
-Adding Slicers and other visuals. 

## Features

### Credit Card Weekly Report
Includes breakdown by Financial quarter , Gender of the card holder , Customer Income Group and the type of card.  
Includes Revenue breakdown details and various KPIs.  

### Credit Card Customer Report
Includes breakdown by Financial quarter , Gender of the card holder , Customer Income Group and the type of card.  
Includes Revenue breakdown details and various KPIs.  


## Insights


## Key Insights from the Dashboards

### 1. Customer and Card Portfolio Health
- **Delinquency is Low:** Only 6.07% of accounts are delinquent, meaning the vast majority (93.93%) of cardholders are in good standing. This indicates strong portfolio quality.
- **High Activation Rates:** 57.47% of cards are activated within 30 days, suggesting effective onboarding/outreach. However, 42.53% may need re-engagement.

### 2. Revenue and Product Mix
- **Blue Cards Dominate Revenue:** Blue category cards generate the highest revenue ($46.13M out of $55.32M total), far eclipsing other card types.
- **Annual Fees Concentration:** Blue cards also lead annual fee collection by a large margin.
- **Fee and Interest Distribution:** Interest income and annual fees are similarly concentrated in Blue cards.

### 3. Customer Segments and Usage
- **Highest Revenue by Use Type:** Swiping cards generates the largest revenue stream ($35M), with chip and online trailing.
- **Business & White-Collar Lead:** Businessmen and white-collar professionals are the largest contributors by customer job.
- **Graduate-Educated Customers Spend More:** Graduates account for $22M in revenue, double the next educational segment.

### 4. Demographic and Geographic Trends
- **Male Customers Spend More:** Across most segments, males contribute more to revenue than females.
- **High-Income Segment Drives Revenue:** Customers classified as high-income generate the majority of the revenue ($22M).
- **Top Revenue States:** Texas (TX), California (CA), and Florida (FL) are the largest contributors by state.

### 5. Quarterly and Weekly Trends
- **Seasonal Revenue Patterns:** The highest revenue and transaction counts occur in Q3—potentially due to seasonal spending.
- **Weekly Fluctuations:** Revenue varies across weeks, with periodic spikes suggesting underlying behavioral or promotional factors.

### 6. Acquisition Costs Insights
- **Blue Cards Have Highest Acquisition Costs:** Acquisition cost for Blue is $0.89M, much higher than others, so focusing on optimizing this could improve margins.

## Actionable Recommendations Based on Insights

- **Customer Engagement:** Re-engage the 42.53% not activated in 30 days through targeted campaigns.
- **Portfolio Growth:** Focus marketing on Blue cards, but also explore promoting other card categories for diversification.
- **Credit Policy:** Monitor and support the small percentage of delinquent accounts to maintain high portfolio quality.
- **Operational Efficiency:** Examine Blue card acquisition strategies to optimize cost vs benefit.
- **Segmentation:** Continue targeting high-value segments (graduates, high income, business professionals).
- **Channel Performance:** Emphasize swipe and chip use features, as these correlate with the most revenue.


## Learning

SQL querying and connecting PostgresSQL to Power BI.
Data connectivity and Updating in Power BI.  
Data modeling in Power BI.  
Designing a Power BI dashboard.  
Using DAX to change numerical data to categorical data.  
