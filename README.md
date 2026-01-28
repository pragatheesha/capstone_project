# Customer Churn Analysis – Capstone Project
## Project Overview

Customer churn is a critical challenge for subscription-based businesses, as losing customers directly impacts revenue and long-term growth. This project performs an end-to-end data analysis on a customer churn dataset to identify key drivers of churn and provide actionable business recommendations to improve customer retention. The project follows a complete data analytics pipeline:
* Data Cleaning → Exploratory Data Analysis → Statistical Analysis → Business Insights

## Objectives
* Clean and prepare raw customer data for analysis
* Understand customer behavior through exploratory analysis
* Identify factors influencing customer churn
* Validate insights using statistical testing
* Segment customers based on churn risk
* Provide data-driven business recommendations

## Project Structure
- customer-churn-analysis
* README.md
* customer_churn.csv
* cleaned_customer_churn.csv
* eda.ipynb
* data_cleaning.ipynb
* analysis.ipynb
* visualizations
* executive_summary.pdf
* technical_report.pdf

## Dataset Description
The dataset contains customer demographic, billing, and service-related information.
  
| Key            | Columns                                    |
|----------------|--------------------------------------------|
| customerid     | Unique customer identifier                 |
| tenure         | Duration of customer relationship (months) |
| monthlycharges | Monthly service charges                    |
| totalcharges   | Total charges paid by the customer         |
| contract       | Type of customer contract                  |
| paymentmethod  | Payment method used                        |
| seniorcitizen  | Senior citizen indicator                   |
| churn          | Whether the customer has churned (Yes/No)  |

The dataset was cleaned and standardized before analysis.

## Data Cleaning
The following steps were performed:
* Standardized column names
* Converted incorrect data types
* Handled missing values using median and mode
* Removed duplicate records
* Created derived features for deeper analysis
* A cleaned dataset (cleaned_customer_churn.csv) was saved for analysis.

## Exploratory Data Analysis (EDA)
* EDA was performed to identify churn patterns and trends:
* Churn distribution analysis
* Monthly charges vs churn
* Tenure vs churn
* Contract type vs churn
* Payment Method vs churn
* Senior Citizen vs Churn
* Correlation analysis of numeric features
* Visualizations were created using Seaborn and Matplotlib.

## Statistical Analysis
To validate insights, statistical tests were applied:
* t-tests to compare churned vs non-churned customers
* t-tests to compare Monthly Charges vs Churn
* t-tests to compare Tenure vs Churn
* Chi-square tests to analyze categorical relationships
* Chi-square tests to analyze Contract Type vs Churn
* Chi-square tests to analyze Payment Method vs Churn
* Correlation analysis for numeric variables
These tests confirmed that pricing, tenure, and contract type significantly influence churn.

## Key Insights
* Customers with higher monthly charges are more likely to churn
* New customers (low tenure) have the highest churn risk
* Month-to-month contracts show significantly higher churn
* Long-term contracts improve customer retention
* Pricing and contract structure are major churn drivers

## Business Recommendations
* Encourage long-term contracts with discounts and incentives
* Target high-risk customers with personalized retention offers
* Improve onboarding experience for new customers
* Review pricing strategies for high-charge customers

## Tools & Technologies

| Python               |                    |
|----------------------|--------------------|
| Pandas               | Data manipulation  |
| NumPy                | Numerical analysis |
| Seaborn & Matplotlib | Data visualization |
| SciPy                | Statistical testing|

## How to Run the Project
* Clone or download the repository
* Install dependencies: pip install pandas numpy seaborn matplotlib scipy
* Run the analysis notebook: jupyter notebook churn_analysis.ipynb

## Conclusion

This project demonstrates how data analytics and statistics can be used to understand customer churn and support data-driven business decisions.The insights and recommendations from this analysis can help businesses reduce churn, improve retention, and increase customer lifetime value.
