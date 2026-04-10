# COVID-19 Trend Analysis & Forecasting

Data analysis and time-series forecasting project analyzing global COVID-19 trends using Python, Plotly interactive visualizations, and Facebook Prophet forecasting models.

---

## Problem Statement

Given data about COVID-19 patients worldwide, this project visualizes the impact of the pandemic, analyzes infection and recovery trends across countries, and forecasts the number of cases expected in the next 7 days based on current trends.

---

## Dataset

**File:** `Covid_19_Clean_Complete.csv`  
**Coverage:** Global — country-level daily data up to July 2020

| Column | Description |
|---|---|
| Date | Date of record |
| Country/Region | Country name |
| Confirmed | Total confirmed cases |
| Deaths | Total deaths |
| Recovered | Total recovered |
| Active | Currently active cases |

---

## Project Objectives

1. Visualize the global spread and impact of COVID-19
2. Compare infection, death, and recovery trends across major countries
3. Build 7-day forecasting models for confirmed cases, deaths, and recoveries

---

## Key Findings

- **US** had the highest confirmed cases and deaths globally as of July 2020
- **India** showed a sharper recovery curve compared to US and Brazil during the same period
- **China** had an early peak and then flattened significantly before other countries peaked
- **Top 10 Deaths:** US, Brazil, UK, Mexico, Italy, France, Spain, India, Iran, Peru
- **Active Cases:** US, Brazil, and India had the most active cases simultaneously
- Prophet forecast showed confirmed cases continuing to rise in the 7-day window with an upper confidence bound significantly above the trend line

---

## Analysis Performed

- Global choropleth map of active cases by country (Plotly)
- Top 10 countries by confirmed cases, deaths, active cases, and recoveries
- Country-level time series comparison: US vs China vs India
- Side-by-side death, recovery, and confirmed case trend lines

---

## Forecasting Models (Facebook Prophet)

Three separate Prophet models were built and evaluated:

| Target | Forecast Period |
|---|---|
| Confirmed Cases | 7 days ahead |
| Deaths | 7 days ahead |
| Recovered | 7 days ahead |

Each model outputs `yhat` (forecast), `yhat_lower` and `yhat_upper` (confidence interval), and trend + seasonality components.

---

## Tech Stack

- **Language:** Python 3
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Plotly, Prophet (Facebook)

---

## Project Structure

```
covid19-trend-analysis/
│
├── Covid 19 analysis.ipynb           # Main code for Time series
├── covid_19_analysis.py              # Full analysis and forecasting code
├── Covid_19_Clean_Complete.csv       # Dataset
└── README.md                         # Project documentation
```

---

## How to Run

1. Clone the repository
```bash
git clone https://github.com/maheshmaddileti-ai/covid19-trend-analysis
```

2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn plotly prophet
```

3. Run the script
```bash
python covid_19_analysis.py
```

> Note: Prophet installation may require additional setup. Run `pip install prophet` if not already installed.

---

## Sample Visualizations

- Interactive choropleth world map (Plotly)
- Point plots comparing US, China, India across Deaths / Recovered / Confirmed
- Prophet forecast plot with confidence intervals
- Bar charts for Top 10 countries by each metric

---

## Author

**Mahesh Maddileti**  
PGP in Data Science & Machine Learning — IntelliPaat (April 2026)  
[LinkedIn](https://linkedin.com/in/maheshmaddileti) | [GitHub](https://github.com/maheshmaddileti-ai)

---

## Certificate

This project was completed as part of the IntelliPaat Post Graduate Program in Data Science & Machine Learning.  
Certificate ID: 31679-462158-209407
