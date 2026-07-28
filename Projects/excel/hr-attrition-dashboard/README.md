# HR Employee Attrition Analysis

## 📌 Overview
An interactive Excel dashboard analyzing employee attrition data to 
identify which departments, roles, and conditions are driving 
employees to leave — and to model what different attrition rates 
would mean for the company going forward.

## 📊 Dataset
IBM HR Analytics Employee Attrition Dataset (Kaggle) — 1,470 employees 
with attrition status, department, job role, overtime, tenure, salary, 
and satisfaction data.
Source: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

## 🛠️ Tools & Skills Used
- Excel Formulas (IFS, XLOOKUP)
- Data Cleaning (duplicate/consistency checks across categorical columns)
- Pivot Tables & Pivot Charts
- What-If Analysis (Data Tables) for attrition rate scenarios
- Slicers for interactivity (Department, Overtime)
- Dashboard design with KPI cards

## 📈 Dashboard Preview
![Dashboard Screenshot](https://github.com/user-attachments/assets/579179d2-7d0a-470c-8986-7bf581679874)

## 🔍 Key Insights
- **Overtime is the single strongest attrition driver:** employees who work overtime leave at a **30.5%** rate, nearly 3x the **10.4%** rate for those who don't — the clearest signal in the entire dataset.
- **New hires are a major flight risk:** employees with 0-2 years of tenure leave at **34.9%**, steadily dropping to **10.4%** for employees with 10+ years — attrition is heavily front-loaded in the first two years.
- **Sales Representatives are the highest-risk role:** a **39.8%** attrition rate, far above every other job role (the next closest is Laboratory Technician at 23.9%).
- **Job satisfaction correlates with staying:** employees who left report an average satisfaction of **2.47** (out of 4), noticeably lower than the **2.78** average for employees who stayed.
- **Sales has the highest departmental attrition** at **20.6%**, compared to **13.8%** in Research & Development — consistent with the Sales Representative role finding above.
- **What-if modeling:** at the current ~16% attrition rate, ~235 of 1,470 employees are projected to leave annually. Reducing attrition to 10% would mean ~147 leavers — a difference of ~88 people retained.

## 🚀 What I'd Improve Next
- Investigate whether overtime is a cause or a symptom (e.g., understaffed teams) by cross-referencing with department
- Build a Power BI version with drill-through by job role and manager
- Add a logistic regression style risk score in Python to rank individual employees by attrition likelihood

## 📁 Files
- `dashboard/HR-Employee-Attrition.xlsx` — final dashboard file
- `Dataset not included in repo — download from the Kaggle link above
