# Emissions Forecast Tool

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-App-ff4b4b?logo=streamlit)
![Data](https://img.shields.io/badge/Data-World%20Bank-orange)
![License](https://img.shields.io/badge/License-MIT-green)

**Problem:** Policy analysts and sustainability teams need to understand how national CO2 emissions are trending and where they are headed.

**Headline result:** ARIMA and ETS models forecast CO2 trajectories for 10 countries with 90% confidence intervals, surfaced in a live Streamlit dashboard using free World Bank Open Data — no API key required.

---

## How to Run

```bash
pip install -r requirements.txt
streamlit run app/app.py
```

---

## Overview

This project downloads CO2 emissions, GDP, and population data from the World Bank API for 10 countries (1990–2022), performs time series analysis, and forecasts emissions trajectories using ARIMA and ETS models. A Streamlit web app provides an interactive interface for country selection, trend comparison, and forecast generation.

---

## Features

- **Live data download** from the World Bank API (free, no registration required)
- **10 countries**: UK, US, China, India, Germany, France, Japan, Brazil, South Africa, Australia
- **Multiple metrics**: total CO2, per capita CO2, GDP, population, carbon intensity
- **ARIMA and ETS forecasting** with configurable horizon and 90% confidence intervals
- **Interactive Streamlit dashboard** with Plotly charts

---

## Data Source

| Source | Coverage | Access |
|---|---|---|
| World Bank Open Data | 1990–2022, 200+ countries | Free API, no registration |

Indicators: EN.ATM.CO2E.KT (CO2 kt), EN.ATM.CO2E.PC (CO2 per capita), NY.GDP.MKTP.CD (GDP), SP.POP.TOTL (Population)

---

## Repository Structure

```
emissions-forecast-tool/
├── app/
│   └── app.py
├── data/clean/
├── notebooks/
│   └── 01_worldbank_pull.ipynb
├── requirements.txt
└── README.md
```

---

## Skills Demonstrated

Python · Pandas · Statsmodels · ARIMA · ETS · Time Series Forecasting · Streamlit · Plotly · World Bank API · Data Visualisation

---

## Author

**Yenlik Gaisina** | Data and Analytics Consultant
[LinkedIn](https://linkedin.com/in/yenlik-gaisina) · [Portfolio](https://gaisina.co.uk)
