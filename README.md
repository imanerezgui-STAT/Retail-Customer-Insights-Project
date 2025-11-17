\# 📊 Retail Customer Insights \& Sales Performance Analytics

End-to-End Data Analysis | Python · PostgreSQL · Power BI



This project delivers a complete analytics workflow on retail customer behavior using real-world style transactional data. It demonstrates the full pipeline required in modern data roles — from data cleaning and preparation, to SQL-based analytics, to interactive BI reporting.



The analysis provides actionable insights on customer segments, purchase behavior, revenue drivers, and geographic patterns to support retail business decision-making.



\## 📁 Project Structure

Retail-Customer-Insights-Project/

│

├── data/

│     └── retail\_customer\_behavior\_raw.csv

│

├── python/

│     └── Retail\_Data\_Cleaning\_and\_Preparation.ipynb

│

├── sql/

│     └── Retail\_Customer\_Insights\_SQL\_Analysis.sql

│

├── powerbi/

│     └── Retail\_Customer\_Insights\_Dashboard.pbix

│

├── reports/

│     ├── Retail\_Customer\_Insights\_PostgreSQL\_Report.pdf

│     └── Final\_Project\_Report.pdf   ← (to be added)

│

├── images/

│     ├── dashboard\_main.png

│     ├── kpi\_section.png

│     ├── category\_chart.png

│     ├── gender\_chart.png

│     ├── seasonality\_chart.png

│     └── location\_map.png

│

└── README.md



\## 🎯 Business Objective



To extract meaningful retail performance insights through customer transaction data, enabling data-driven decisions in:



Product assortment strategy



Customer segmentation \& marketing



Seasonality planning



Revenue optimization



Regional sales focus



\## 📦 Dataset Overview



The dataset contains 3,900 retail transactions across U.S. regions.



Key Fields

Column	Description

customer\_id	Unique customer identifier

age	Age of customer

gender	Male / Female

item\_purchased	Specific item bought

category	Product category

purchase\_amount\_usd	Transaction value

location	U.S. state

size	S, M, L

color	Purchased item color

season	Season of purchase

review\_rating	Customer rating (1-5)

subscription\_status	Yes/No

shipping\_type	Shipping method

discount\_applied	Yes/No

promo\_code\_used	Yes/No

previous\_purchases	Count of past purchases

\## 🧹 1. Data Cleaning (Python)



Python cleaning was performed using:



pandas for data loading \& transformation



missing value checks



type corrections



column renaming for SQL \& BI compatibility



outlier review



pre-export validation



The cleaned dataset was saved for SQL \& Power BI under:



data/retail\_customer\_behavior\_raw.csv





Notebook:



python/Retail\_Data\_Cleaning\_and\_Preparation.ipynb



\## 🗄 2. Analytical Processing (PostgreSQL)



The cleaned dataset was imported into PostgreSQL for structured querying and KPI analysis.



SQL file:



sql/Retail\_Customer\_Insights\_SQL\_Analysis.sql



Key Queries Executed



Total revenue



Total transactions



Average basket value (ABV)



Revenue by category



Transactions by gender



Seasonality analysis



Geographic transaction distribution



Full SQL report:



reports/Retail\_Customer\_Insights\_PostgreSQL\_Report.pdf



\## 📈 3. Business Intelligence Dashboard (Power BI)



Power BI transforms the SQL \& Python insights into an interactive visual analytics experience.



Dashboard file:



powerbi/Retail\_Customer\_Insights\_Dashboard.pbix



\### 🔧 DAX Measures Used

Total Revenue = SUM('retail\_data'\[purchase\_amount\_usd])



Total Transactions = COUNTROWS('retail\_data')



ABV = DIVIDE(\[Total Revenue], \[Total Transactions])



\### 🖥 Dashboard Overview

⭐ Executive KPI Cards



Total Revenue



Total Transactions



Average Basket Value (ABV)



⭐ Performance Visuals



Revenue by category



Transactions by gender



Revenue by season



Geographic sales distribution (map)



\### 🖼 Dashboard Screenshots

Component	Screenshot

Full Dashboard	images/dashboard\_main.png

KPI Section	images/kpi\_section.png

Category Chart	images/category\_chart.png

Gender Distribution	images/gender\_chart.png

Seasonality	images/seasonality\_chart.png

US Map	images/location\_map.png

\## 📊 Summary of Insights

✔ Clothing generates the highest total revenue



The category consistently outperforms all others.



✔ Male customers represent the majority of transactions



Marketing campaigns can be gender-targeted accordingly.



✔ Spring and Fall seasons deliver the strongest revenue



Useful for inventory planning and seasonal promotions.



✔ Geographic analysis shows strong performance across central and western states



Helps identify priority expansion areas.



✔ Customer spending is stable



ABV remains constant, supporting predictable revenue forecasting.



\## 🚀 Final Recommendations



Increase inventory in top-performing categories (Clothing \& Accessories)



Design gender-specific marketing flows (higher male conversion)



Plan major promotional campaigns during Spring and Fall



Prioritize logistics optimization for high-transaction states



Leverage subscription programs to increase customer retention



\## 🧪 Technologies Used



Python (pandas, numpy) – Data cleaning



PostgreSQL – Analytical queries



Power BI – Interactive dashboard



GitHub – Version control \& portfolio presentation



\## 📬 Contact



For questions or collaboration opportunities:



Imane Rezgui

Data Analyst | Business Analyst | Finance \& Retail Analytics

Email: imane.rezgui.pro@gmail.com

LinkedIn: www.linkedin.com/in/imane-rezgui

