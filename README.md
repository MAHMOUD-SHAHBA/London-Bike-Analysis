# London Bike Analysis 🚴‍♂️📊

## Project Overview
This project analyzes **London’s bike-sharing data** to understand **rental patterns, seasonal trends, weather impact, and temporal behavior**.  
The goal is to uncover actionable insights for **optimizing bike allocation** and to create an **interactive dashboard in Tableau**.

**Key Features:**
- Data cleaning and preprocessing
- Feature engineering: hour, weekday, month, year, weekend label
- Exploratory Data Analysis (EDA) with Python (pandas, matplotlib, seaborn)
- Professional Tableau dashboard with KPIs, line charts, bar charts, donut charts, heatmaps, and maps

---

## Dataset
- Source: London Bike Sharing Dataset


**Data Cleaning & Feature Engineering Steps:**
1. Rename columns for clarity
2. Convert timestamps to datetime objects
3. Normalize humidity values (`/100`)
4. Map numeric codes to readable labels (season, weather)
5. Create new features: `hour`, `weekday`, `month`, `year`, `is_weekend_label`

---

## Exploratory Data Analysis (EDA)
**Visualizations in Python:**
- Average bike rentals by season (with weekend hue)
- Rentals distribution by weather condition
- Hourly rental heatmap
- Scatter plot of temperature vs rentals

**Insights:**
- Peak rentals occur during **summer weekdays**
- Weather impacts demand significantly; rainy or stormy days reduce rentals
- Morning and evening rush hours show highest usage
- Rentals correlate positively with temperature

---

## Tableau Dashboard
**Interactive, executive-ready dashboard** with:
- **KPIs:** Total Rentals, Avg Daily Rentals, Peak Rentals, Avg Temperature
- **Trends:** Line charts for time series, rolling average area chart
- **Patterns:** Bar charts for season/weekend and weather
- **Proportions:** Donut chart for seasonal distribution
- **Usage Heatmap:** Hour × Weekday
- **Map Visualization:** Bike station usage (if latitude/longitude available)

**Filters included:** Year, Season, Weather, Weekday/Weekend

---


## Project Structure
London-Bike-Analysis/
│
├─ README.md
├─ london_bikes_clean.xlsx # Cleaned dataset
├─ plots/ # Python-generated plots
│ ├─ rentals_by_season.png
│ ├─ rentals_by_weather.png
│ └─ heatmap_hour_weekday.png
├─ notebooks/ # Optional Jupyter notebooks
├─ Tableau/ # Tableau workbook files (.twbx)
└─ scripts/ # Python scripts for EDA & cleaning