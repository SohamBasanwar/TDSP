# Explorer Transportation Data Science Project (TDSP)
**NYC Motor Vehicle Collisions — Exploratory + Time-Series Analysis**

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-EDA%20%26%20Cleaning-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualizations-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Stats%20Plots-purple)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## Overview
This project is part of the **Explorer Transportation Data Science Project**, where I analyzed the **NYC OpenData Motor Vehicle Collisions – Crashes** dataset.  
The goal is to explore crash patterns, address data quality/ethics, and use time-series analysis to understand how crashes change over time.

## What I Did (Milestones)
### Milestone 1 — Data Preparation
- Set up a Google Colab environment and imported core libraries.
- Loaded and inspected the NYC collisions dataset.
- Used `head()`, `describe()`, `sum()`, `isnull()`, and `value_counts()` to understand structure and basic stats.

### Milestone 2 — Data Ethics + Pre-Processing + EDA
- Identified missing values and discussed how reporting bias can affect conclusions.
- Visualized top contributing factors to crashes.
- Visualized vehicles most frequently involved in collisions.
- Suggested practical improvements for data collection and labeling.

### Milestone 3 — Time Series Analysis
- Converted crash timestamps to datetime.
- Aggregated crashes by hour/day to detect recurring trends.
- Built plots showing when crashes peak during the day.

## Key Findings
- **Missing Data is heavy** in vehicle type and contributing factor columns.  
  This suggests inconsistent reporting and must be handled carefully before modeling.
- **Top contributing factors (excluding "Unspecified")**:
  1. Driver Inattention/Distraction  
  2. Failure to Yield Right-of-Way  
  3. Backing Unsafely
- **Most involved vehicle categories**:
  - Sedans  
  - Passenger vehicles  
  - SUVs / Station wagons  
- **Crash peak time:** **~3 PM to 6 PM**, matching evening rush hour traffic.

## Tech Stack
- **Python**
- **Pandas** — cleaning + analysis  
- **Matplotlib / Seaborn** — visualizations  
- **Google Colab** — execution environment

## Dataset
Source: **NYC OpenData — Motor Vehicle Collisions (Crashes)**  
The dataset contains reported collisions in NYC with fields like:
- Location (borough, street, lat/long)
- Crash time/date
- Vehicle types involved
- Contributing factors
- Injuries and fatalities

## How to Run
### Option 1: Google Colab (recommended)
1. Open the notebook in Colab.
2. Upload the dataset CSV to your Google Drive.
3. Update the file path inside the notebook.
4. Run cells top-to-bottom.

### Option 2: Local Jupyter
```bash
git clone <your-repo-url>
cd TDSP
pip install -r requirements.txt
jupyter notebook
