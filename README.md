# 🚲 Nextbike Stirling Utilisation Analysis

> A data-driven project to improve bike-sharing efficiency and sustainability using Python and Power BI

---

## 🎯 Business Problem

Stirling Council has invested over £11 million in cycling infrastructure to promote active travel and reduce transport emissions. However, the Nextbike scheme remains underutilised.

Despite:
- 160 bikes available across the city
- Strong demand during peak hours

The system averages only ~78 trips per day.

**The challenge:**
Why is the system underperforming — and how can we fix it without additional investment?

---

## 📊 Dataset

- 140,689 bike trips (2018–2023)
- Features include:
  - Trip timestamps (hour, day, month, year)
  - Trip duration
  - Start and end stations
  - Location-based data (station coordinates)

---

## What I Actually Did

### Data Cleaning & Preparation

Audited and cleaned raw trip data using Python (Pandas):
- Handled missing and inconsistent values
- Standardised time-based features (hour, day, month)
- Created structured datasets for analysis and reporting

### Feature Engineering

Engineered key variables to capture system behaviour:
- **Net Flow** = Rentals – Returns → Identifies station-level surplus and shortages
- **Peak Demand Indicators** → Highlighted high-demand time windows (3–5 PM)
- **Redistribution Priority Metrics** → Ranked stations based on imbalance severity

### Exploratory Data Analysis (EDA)

Performed detailed analysis using Python:
- Time-series analysis → usage trends across years
- Hourly patterns → peak demand identification
- Daily trends → weekday vs weekend behaviour
- Correlation analysis → relationship between trip starts and ends

### Power BI Dashboard Development

Built an interactive dashboard to communicate insights:
- Time-series visualisation of trip demand
- Station-level inflow/outflow analysis
- Identification of surplus vs shortage locations
- Visualisation of redistribution strategies

> This step translates raw analysis into decision-making tools for stakeholders.

---

## Key Findings

### 1. Demand Exists — But Is Poorly Served
- Strong peak demand between 3 PM – 5 PM
- Higher usage on weekdays
- Demand driven by commuting and student movement

### 2. Core Issue: Spatial Imbalance

Net flow analysis revealed:
- University stations → consistent shortages
- City centre & transport hubs → bike surplus

➡️ Bikes accumulate in low-demand areas and are unavailable where needed

### 3. Not a Demand Problem

The system is not failing due to lack of interest.

Instead:
- Users cannot access bikes when needed
- Availability issues directly reduce usage

---

## 💡 Solution

### Targeted Redistribution Strategy
- Move 20–30 bikes daily
- Timing: 2–3 PM (before peak demand)
- From surplus locations → university stations

This ensures availability during high-demand periods.

### Behavioural Interventions (EAST Framework)

Encourage users to help rebalance the system:
- **Easy** → Show nearby high-demand stations
- **Attractive** → Rewards (discounts / loyalty points)
- **Social** → CO₂ savings feedback
- **Timely** → Nudges during peak return hours

---

## 🌱 Impact

Over 5 years:
- ~44.5 tonnes of CO₂ saved

With optimisation:
- Increased bike usage
- Reduced car dependency
- Improved return on £11M infrastructure investment
- Supports Net Zero 2045 targets

---

## 🚀 Why This Project Matters

This project demonstrates:
- How data can uncover hidden inefficiencies in real systems
- The importance of supply-demand alignment in operations
- How small, low-cost interventions can drive meaningful impact
- The value of combining data analysis + behavioural science

---

## 📓 View the Full Analysis

Click [`nextbike_stirling_analysis.ipynb`](https://github.com/Imran3285/nextbike-stirling-PowerBI-analysis/blob/main/nextbike_stirling_analysis.ipynb)
to explore the full Python analysis pipeline, including data cleaning, EDA, and feature engineering.

---

## 📊 Dashboard

Power BI dashboard available here:
[`PowerBI visuals`](https://github.com/Imran3285/nextbike-stirling-PowerBI-analysis/tree/main/PowerBI%20visuals)

Includes:
- Demand trends
- Station imbalance analysis
- Redistribution strategy visuals

---

## Project Structure
```
├── PowerBI visuals/
├── nextbike_data_sample.csv
├── nextbike_stirling_analysis.ipynb
├── nextbike_stirling_utilisation_report.pdf
└── README.md
```

---

## Reproducing the Analysis
```bash
git clone https://github.com/Imran3285/nextbike-stirling-PowerBI-analysis.git
cd nextbike-stirling-PowerBI-analysis
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook
```

Run all cells in the notebook to reproduce results.

---

## Stack

`Python` · `Pandas` · `NumPy` · `Power BI` · `DAX Query` · `Matplotlib` · `Seaborn` · `Jupyter`

---

## Author

**Muhammad Imran**
