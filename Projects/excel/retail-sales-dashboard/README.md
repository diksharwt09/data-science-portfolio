# Retail Sales Performance Dashboard

## 📌 Overview
An interactive Excel dashboard analyzing retail sales data to uncover 
trends in revenue, profit, and customer behavior across regions and 
product categories.

## 📊 Dataset
Sample Superstore Dataset (Kaggle) — ~10,000 orders including sales, 
profit, region, category, customer segment, and shipping details.
Source: https://www.kaggle.com/datasets/vivek468/superstore-dataset-final

## 🛠️ Tools & Skills Used
- Excel Formulas (IF/IFS, YEAR, TEXT)
- Data Cleaning (Remove Duplicates, date formatting checks)
- Pivot Tables & Pivot Charts
- Slicers for interactivity
- Dashboard design with KPI cards

## 📈 Dashboard Preview
![Dashboard Screenshot](https://github.com/user-attachments/assets/0742d79f-a42c-42ce-a04c-683e8dcc6579)

## 🔍 Key Insights
- **Furniture is a margin trap:** despite generating the 2nd-highest sales (~$742K), Furniture returns only a 2.5% profit margin — far below Office Supplies (17%) and Technology (17.4%). Two sub-categories, Tables and Bookcases, are actually losing money (-8.6% and -3.0% margin), likely due to heavy discounting.
- **West is the strongest region overall:** highest sales ($725K) and highest profit margin (14.9%), while Central lags on both fronts (7.9% margin) despite comparable order volume — worth investigating regional discount or pricing policy.
- **Copiers and Paper are the hidden profit stars:** despite modest sales, they carry the highest margins in the dataset (37% and 43% respectively) — worth promoting or bundling more.
- **Revenue is not overly concentrated:** the top 10 customers account for only ~6.7% of total sales, meaning the business isn't overly reliant on a handful of accounts — a healthy sign.
- **Technology leads in raw sales** ($836K) and holds a strong margin (17.4%), making it the most balanced category — high volume and healthy profitability together.

## 🚀 What I'd Improve Next
- Analyze the impact of discount level directly on the Tables/Bookcases losses to see if a discount cap would fix the margin
- Build a Power BI version with drill-through by state, not just region
- Add a forecast trend using moving averages for next-quarter sales

## 📁 Files
- `dashboard/Retail_Sales_Dashboard.xlsx` — final dashboard file
- Dataset not included in repo — download from the Kaggle link above
