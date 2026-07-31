# Netflix Content Strategy Dashboard

## 📌 Overview
An interactive Power BI dashboard analyzing Netflix's content catalog 
to understand how their content strategy has evolved over time — what 
they've added, from where, and in what format.

## 📊 Dataset
Netflix Movies and TV Shows dataset (Kaggle) — ~8,800 titles including 
type, country, release year, date added, rating, and duration.
Source: https://www.kaggle.com/datasets/shivamb/netflix-shows

## 🛠️ Tools & Skills Used
- Power Query (Trim, Clean, Replace Values, Split Column by Delimiter, Extract Text Before Delimiter, Conditional Columns, Remove Errors)
- DAX Measures (DISTINCTCOUNT, CALCULATE, DIVIDE)
- Card, Line Chart, Bar Chart, and Clustered Column Chart visuals
- Slicers (Release Year range, Content Type)

## 📈 Dashboard Preview
![Dashboard Screenshot](width="1430" height="796" alt="Screenshot 2026-07-31 184557" src="https://github.com/user-attachments/assets/1a431840-d67a-45d0-b981-82056b9b9f2e" />)

## 🔍 Key Insights
- **Netflix's catalog grew explosively after 2015:** content additions were nearly flat through 2014, then rose sharply, peaking around 2019 before a slight pullback — reflecting Netflix's aggressive content investment phase in the late 2010s.
- **Movies dominate the catalog:** roughly two-thirds of titles are Movies (~6,100) versus one-third TV Shows (~2,700), despite TV Shows often driving more subscriber engagement.
- **The United States leads content origin by a wide margin**, followed by India and the United Kingdom — with India's strong second-place position reflecting Netflix's international expansion push.
- **TV-MA is the most common content rating** across both Movies and TV Shows, indicating the catalog skews toward mature audiences.
- **Data quality mattered as much as analysis:** the raw dataset contained shifted/misaligned rows (dates appearing in rating fields and vice versa) — these were identified and cleaned during the Power Query stage rather than left to distort the visuals.

## 🚀 What I'd Improve Next
- Split the `listed_in` (genre) column the same way `country` was split, to build an accurate genre-level breakdown
- Add a measure comparing average Movie duration vs. TV Show season count over time
- Build a second page comparing content added by Netflix Originals vs. licensed content, if that data were available

## 📁 Files
- `dashboard/Netflix_Titles.pbix` — final Power BI report
- `data/netflix_titles.csv` — raw dataset<img 
