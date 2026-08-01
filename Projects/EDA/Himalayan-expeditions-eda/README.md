# Himalayan Expeditions — Exploratory Data Analysis

## 📌 Overview
An exploratory data analysis of decades of Himalayan mountaineering 
expedition data, examining how success rates, safety, team size, and 
climbing nations have changed over time — and testing whether 
supplemental oxygen genuinely improves outcomes.

## 📊 Dataset
The Himalayan Database — expedition and peak records for Nepal Himalaya 
climbs. This project used `exped.csv` (~11,400 expedition-level records) 
and `peaks.csv` (~480 peak records, merged in for peak names).
Source: https://mavenanalytics.io/data-playground/himalayan-expeditions

## 🛠️ Tools & Skills Used
- Python (pandas, matplotlib, seaborn) in Jupyter Notebook
- Data inspection (`.info()`, `.isnull().sum()`) before cleaning
- Groupby aggregation and rate calculations
- Table merging (`.merge()`) to join expedition and peak data
- Correlation analysis and heatmap visualization
- Identifying and correcting a small-sample-size distortion
- Identifying and correcting a confounding variable in a group comparison

## 📈 Notebook Preview
![Success and Death Rate by Decade](screenshots/success_death_rate.png)

## 🔍 Key Insights
- **Climbing has gotten dramatically safer and more successful since 1950:** success rates rose from ~34% in the 1950s to over 70% in the 2020s, while death rates fell from a 1970 peak of ~2.7% to under
 1% today. *(Pre-1950 data was excluded due to very small sample sizes — as few as 10 expeditions in the 1920s.)*
- **Oxygen's real safety benefit only became visible after controlling for peak difficulty.** Across all peaks, oxygen users had far higher success rates (~80% vs ~45%) but nearly identical death rates to non-oxygen climbers — a misleading result caused by oxygen being used disproportionately on the most extreme peaks. Isolating Everest alone revealed the true effect: non-oxygen climbers succeed only ~6% of the time (vs ~80% with oxygen) and face a notably higher death rate (~2.5% vs ~1.5%).
- **Expedition teams have shrunk significantly since the 1970s** — average team size peaked at ~10 members in the 1970s ("siege-style" expeditions) and declined to ~5 by the 2010s.
- **The USA, Japan, and UK have sent the most expeditions historically.**
- **Annapurna I and Dhaulagiri I rank among the deadliest peaks** (minimum 20 expeditions), consistent with their well-known reputations in real-world mountaineering.

## 🚀 What I'd Improve Next
- Use `members.csv` (individual climber records, not used in this pass) to analyze outcomes by age, nationality, or hired vs. non-hired status
- Test whether the oxygen effect holds on other 8000m peaks besides Everest
- Build an interactive version of these charts in Power BI or Tableau

## 📁 Files
- `notebook/Himalayan_EDA.ipynb` — full analysis notebook
- Raw data (`exped.csv`, `peaks.csv`) not included in this repo — download from the Maven Analytics link above
