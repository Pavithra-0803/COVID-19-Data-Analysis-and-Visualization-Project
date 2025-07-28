# 🦠 COVID-19 India Data Analysis Project

This project provides an in-depth analysis of the COVID-19 situation in India using real-world data. The analysis includes state-wise comparisons, trend visualizations, and calculated metrics like recovery and mortality rates to understand the pandemic’s evolution and impact.

---

## 📌 Objectives

- Load and clean COVID-19 datasets specific to India.
- Analyze daily trends in confirmed, cured, and death cases.
- Visualize state-wise active cases and death counts.
- Calculate recovery and mortality rates.
- Identify top affected states and compare time series trends.
- Analyze vaccination data alongside case statistics.

---

## 📂 Dataset Sources

- **COVID-19 India Cases Dataset**: Contains daily confirmed, cured, and death counts by state.
- **Vaccination Dataset**: Contains state-wise vaccine distribution data.

---

## 🧪 Technologies Used

- **Python 3**
- **Pandas** – data manipulation
- **NumPy** – numerical operations
- **Matplotlib & Seaborn** – static data visualizations
- **Plotly** – interactive plots
- **Jupyter Notebook**

---

## 📊 Project Workflow

### 1. Data Import and Exploration

- Loaded COVID-19 case data and vaccination data from CSV files.
- Inspected data with `.head()`, `.info()`, and `.describe()`.

### 2. Data Cleaning

- Dropped irrelevant columns such as `Sno`, `Time`, `ConfirmedIndianNational`, and `ConfirmedForeignNational`.
- Created a new column `Active_cases` using:


### 3. State-wise Aggregation

- Created a pivot table to summarize max `Confirmed`, `Deaths`, and `Cured` by state.
- Calculated:
- **Recovery Rate** = `(Cured / Confirmed) * 100`
- **Mortality Rate** = `(Deaths / Confirmed) * 100`
- Sorted data by `Confirmed` cases in descending order.

### 4. Visualizations

- **Bar Plot** of Top 10 states with the most active cases.
- **Bar Plot** of Top 10 states with the highest deaths.
- **Line Plot** showing the trend of active cases over time in key states like:
- Maharashtra
- Karnataka
- Kerala
- Tamil Nadu
- Uttar Pradesh

- Used Plotly for interactive visualizations (e.g., trend analysis).

### 5. Time Series Analysis

- Converted the `Date` column to datetime format.
- Extracted the `month` for temporal analysis.
- Created monthly trends using seaborn’s line plots.

---

## 📈 Sample Insights

- **Maharashtra** had the highest number of confirmed and death cases.
- **Kerala** showed consistently high active cases with strong recovery.
- **Top states** with active cases and deaths were visualized to show their trends clearly.
- **Recovery rates** were high in most states but mortality varied depending on healthcare and response.

---



