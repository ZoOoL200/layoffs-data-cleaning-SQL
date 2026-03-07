# 📊 World Layoffs - Exploratory Data Analysis (SQL)

## Project Overview
This phase of the project focuses on **Exploratory Data Analysis (EDA)**. After cleaning the global layoffs dataset, the goal is to extract meaningful insights, identify trends, and rank the impact of layoffs across different dimensions such as time, geography, and industry.

## Analysis Objectives
The analysis aims to answer several key business questions:
* What is the total timeframe covered by the data?
* Which countries and industries suffered the most layoffs?
* How do layoffs trend annually and quarterly?
* Is there a correlation between funds raised and the number of layoffs?
* Which companies experienced a total shutdown (100% layoffs)?

---

## Technical Skills Applied
* **Advanced CTEs:** Used for multi-step aggregations and complex filtering.
* **Window Functions (`DENSE_RANK`):** Applied to rank countries, industries, and companies based on layoff volume.
* **Time-Series Analysis:** Using `YEAR()`, `QUARTER()`, and `STR_TO_DATE` for temporal trends.
* **Data Aggregation:** Extensive use of `SUM()`, `COUNT()`, `AVG()`, and `GROUP BY`.

---

## Key Insights & Query Highlights

### 1. Global Rankings (Top 5)
The project identifies the top 5 entities globally and per year for:
* **Countries:** Ranking by total employees laid off.
* **Industries:** Identifying the hardest-hit sectors.
* **Companies:** Highlighting specific organizations with massive workforce reductions.

### 2. Temporal Trends
* **Yearly Impact:** Ranking years based on the total volume of layoffs.
* **Worst Quarters:** Identifying which quarter of each year saw the highest layoff activity.

### 3. Company Shutdowns
A specialized analysis of companies that laid off **100%** of their workforce, categorized by:
* Total count of shutdowns per year.
* Top countries and industries prone to complete company failures.

### 4. Financial Analysis
* Exploring the relationship between `funds_raised_millions` and the average `total_laid_off` to see if high funding prevents or correlates with large layoffs.

---

## Summary of Findings
The analysis reveals significant spikes in layoffs during specific years and quarters, with certain industries (like Tech and Finance) and specific regions showing higher vulnerability. The use of ranking functions allowed for a clear view of the most impacted sectors in the global economy.

**Author:** Ahmed Rabie
