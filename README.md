# Bank Loan Report

### Dashboard Link : https://app.powerbi.com/view?r=eyJrIjoiMmIzZGE1MDctODE2ZS00ZTBiLWE5NDctOTFjYTNmZTliZDU3IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9

## Problem Statement

This project aims to create a comprehensive dashboard to track and analyze key metrics related to loan applications, disbursements, repayments, and borrower characteristics. By calculating essential KPIs like total loan applications, funded amounts, amounts received, interest rates, and debt-to-income (DTI) ratios, the dashboard will enable the bank to track month-to-date (MTD) data and month-over-month (MoM) changes. The dashboard will feature various visualizations such as trend charts, regional analysis maps, loan term distributions, and borrower profile breakdowns, providing insights into lending activity, borrower financial health, and loan portfolio performance. The goal is to provide an intuitive and efficient tool for monitoring and making informed decisions about the bank’s lending practices.

 ## Power BI Features Used:

Power Query

DAX Measures

Visualizations: Line, Bar, Filled Map, Tree Map, Donut chart, Cards

### Steps followed 

#### Step 1: Loaded Data into Power BI
Connected to the SQL Server database by opening Power BI Desktop and selecting Get Data → SQL Server.

Choose Import mode to load the data from the relevant tables.


#### Step 2: Opened Power Query Editor
Opened Power Query Editor.

In the View tab, enabled the following options under Data Preview:

Column Distribution

Column Quality

Column Profile

#### Step 3: Modified Column Profiling Settings
By default, the profile was based on the first 1000 rows. Changed this to "Column profiling based on entire dataset" for a complete view of the data.

#### Step 4: Data Cleaning and Transformation
Checked for any blank values, duplicates, or mistakes in the data.

Modified data types of necessary fields to ensure consistency.

After completing these transformations, the data was ready for reporting.

#### Step 5: Validated Data with SQL Queries
Before building the report, ran all necessary SQL queries in SQL Server Management Studio (SSMS) to get exact numbers.

Used these results to cross-check the data reflected in Power BI visuals for accuracy.

#### Step 6: Created Date Table and Relationships
Created a Date Table using DAX in Power BI.

Marked the Date Table as a Date Table and created a relationship between it and the Bank Loan Table using the issue date field.


#### Step 7: Identified Key Metrics and KPIs
Listed the Key Performance Indicators (KPIs) and business questions that needed to be answered in the report, such as:

Total Loan Applications

Total Funded Amount (including MTD and MoM trends)

Total Amount Received (including MTD and MoM trends)

Average Interest Rate (overall, MTD, and MoM)

Average Debt-to-Income (DTI) Ratio (overall, MTD, and MoM)


#### Step 8: Created Good Loan Vs Bad Loan comparison KPIs
Loan Application Percentage
 
Loan Applications

Loan Funded Amount

Loan Total Received Amount

![Snap_1](https://github.com/user-attachments/assets/5e4e126f-fda2-4787-afe9-a97c205dc63a)


#### Step 9: Created Visualizations in Power BI
Built the following charts to visualize the data:

Line Chart: Monthly trends by issue date

Filled Map: Regional analysis by state

Donut Chart: Loan term distribution

Bar Chart: Employment length distribution

Bar Chart: Loan purpose breakdown

Tree Map: Impact of home ownership on loan applications

![Snap_2](https://github.com/user-attachments/assets/5e4e126f-fda2-4787-afe9-a97c205dc63a)

#### Step 10: Organized Report Layout
Created the Summary tab with KPIs.

Placed all visualizations in the Overview tab.

Designed the details tab to give a consolidated summary of business insights.


![Snap_3](https://github.com/user-attachments/assets/5e4e126f-fda2-4787-afe9-a97c205dc63a)
