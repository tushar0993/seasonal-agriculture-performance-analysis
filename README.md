# Seasonal Agriculture Performance Analysis

**Major Project — VOIS AICTE Data Analytics Program (Batch 1, 2026–2027)**

## Overview

This project analyzes farm-level agricultural data to understand how performance — yield, water use, and profitability — varies across India's three cropping seasons: Kharif, Rabi, and Zaid. Raw agricultural data doesn't clearly show why performance shifts season to season, so this analysis digs into the environmental, resource-use, and economic factors driving those differences.

## Dataset

- **File:** `seasonal_agriculture_performance_dataset.csv`
- **Records:** 4,000 farms
- **Coverage:** 8 states (Andhra Pradesh, Maharashtra, Telangana, Karnataka, Gujarat, Tamil Nadu, Punjab, Madhya Pradesh), 8 crops (Wheat, Maize, Pulses, Rice, Cotton, Chilli, Groundnut, Sugarcane), 3 seasons
- **Fields:** environmental conditions (rainfall, temperature, humidity, soil pH/moisture), farming inputs (fertilizer, pesticide, irrigation method, seed quality), and outcomes (yield, production, cost, revenue, profit, water usage/efficiency, disease-pest risk)

## Tools Used

- Python 3
- Pandas & NumPy — data cleaning and aggregation
- Matplotlib & Seaborn — univariate, bivariate, and multivariate visualization

## Approach

1. Initial data understanding and quality checks
2. Data cleaning (missing values, duplicates, categorical consistency)
3. Descriptive statistical analysis
4. Univariate, bivariate, and multivariate visual analysis
5. Season-by-season comparison of key performance metrics
6. Key findings and recommendations

## Key Findings

- **Kharif is the most profitable season; Zaid is the weakest.** Kharif has the highest average rainfall, yield, and profit margin (~25%). Zaid — the driest, hottest season — runs an overall negative profit margin, with roughly 6 in 10 Zaid farms operating at a loss versus about 4 in 10 in Kharif.
- **Water efficiency doesn't track water usage.** Flood irrigation uses the most water per farm (~8,026 m³ on average) but is the least efficient (3.44 tonnes per 1000 m³). Drip irrigation is clearly more efficient than Sprinkler or Flood (6.27 vs 4.67 vs 3.44 t/1000m³) among actively managed methods.
- **Yield tracks water efficiency more than fertilizer or nutrients.** The correlation between yield and water efficiency is notably stronger than yield's correlation with Nitrogen, Phosphorus, or Potassium application.
- **Sugarcane yields dominate every season by a wide margin** — yield should be read per-crop, not as one combined distribution.
- **Disease and pest risk peaks in Kharif** (wettest, most humid season) and is lowest in Zaid, consistent with pest/disease pressure rising with rainfall and humidity.
- **Profit is driven by revenue and yield, not farm size** — farm area has a comparatively weak correlation with profit, suggesting smaller, well-managed farms can perform on par with larger ones.

## Recommendations

- Re-evaluate Zaid-season cultivation — review crop choice, irrigation method, and input costs given its negative margin and high share of loss-making farms.
- Encourage drip irrigation where feasible, especially outside Kharif, given its stronger water efficiency and yield outcomes.
- Strengthen pest and disease monitoring during Kharif, when disease/pest risk peaks alongside rainfall and humidity.
- Base crop diversification decisions on per-crop yield data, since yield and profit track crop choice and resource efficiency more than farm size.

## Repository Contents

| File | Description |
|------|-------------|
| `Seasonal_Agriculture_Performance_Data_Analytics.ipynb` | Full analysis notebook |
| `DATASET.csv` | Source dataset |
| `Major_Project_Seasonal_Agriculture_Performance_Analysis.pdf` | Project brief |
| `Tushar_STU6a6a3132c25111785344306.PPTX` | Presentation summary |

## Author

**Tushar** — Netaji Subhas University Of Technology
