# Retail Customer Insights Project

## Introduction


## Data Dictionary
| Variable | Business Meaning |
|-----------|------------------|
| Customer ID | Unique customer identifier used to link transactions and compute KPIs (frequency, retention, CLV, RFM). |
| Age | Customer age used for demographic segmentation, cohort analysis, and targeting. |
| Gender | Customer gender for segmentation and personalized marketing analysis. |
| Item Purchased | Product/SKU purchased; used for product-level trends, attachment, and inventory insights. |
| Category | High-level product grouping for assortment optimization, margin mix, and performance tracking. |
| Purchase Amount (USD) | Monetary value of the transaction (net of discounts if available); core input for revenue and ABV. |
| Location | Store/mall/city of purchase; used for geographic sales analysis and logistics planning. |
| Size | Product size variant; supports demand forecasting by variant and inventory allocation. |
| Color | Product color attribute; used for style preference and seasonal assortment analysis. |
| Season | Season of purchase (e.g., Winter, Summer); used for seasonality and promotional timing. |
| Review Rating | Post-purchase satisfaction score (1–5); proxy for product quality and CX. |
| Subscription Status | Customer enrollment in loyalty/membership; indicator for retention propensity and recurring value. |
| Shipping Type | Fulfillment method (e.g., Standard, Express, Free); affects delivery cost, SLA, and conversion. |
| Discount Applied | Indicates presence/amount of discount on the transaction; measures promotion effectiveness and margin impact. |
| Promo Code Used | Flag/code for applied promotion; used to attribute campaign performance and price sensitivity. |
| Previous Purchases | Count of historical purchases prior to this transaction; input to RFM/loyalty scoring. |
| Payment Method | Tender type (e.g., Cash, Card, Wallet); informs checkout optimization and payment costs. |
| Frequency of Purchases | Shopping cadence (e.g., Weekly, Monthly) or derived frequency metric; measures engagement level. |



🧹 Data Cleaning and Preparation – Customer Shopping Behavior Analysis
Objective

Prepare the raw dataset for analysis by correcting formats, standardizing column names, and handling missing or inconsistent values. The goal is to ensure data quality and analytical reliability before KPI design and dashboarding.

Steps Performed

Column Standardization

Converted all column names to lowercase snake_case.

Removed extra spaces and special characters for compatibility across SQL, Python, and BI tools.

Data Type Correction

Automatically converted columns that are mostly numeric (≥90 % numeric values) into numeric data types.

Protected identifier columns (e.g., customer_id) from conversion to preserve text formatting.

Parsed any date/time fields detected by name.

Categorical Cleaning

Trimmed spaces and normalized yes/no values into consistent boolean (True/False) format.

Retained categorical attributes (e.g., region, color, size) as text.

Duplicate Removal

Detected and removed exact duplicate rows to avoid double counting in KPIs.

Missing-Value Handling (Imputation Policy)

Default mode: keep missing values (IMPUTE=False) for transparency and manual review.

Optional mode (IMPUTE=True):

Numeric → median

Date/time → most frequent date

Categorical → mode or “Unknown”

Outlier Detection (Not Removal)

Calculated z-scores for numeric columns and flagged records where |z| > 4 for further investigation.

Data Dictionary Creation

Generated a CSV summary with each column’s type, non-null count, and number of unique values.

Outputs Produced

customer_shopping_behavior_clean.csv → cleaned dataset ready for analysis.

customer_shopping_behavior_data_dictionary.csv → schema overview.

Key Outcome

The dataset is now consistent, analysis-ready, and suitable for exploratory analysis, KPI computation, and dashboard integration in Power BI or Python visualization libraries.
