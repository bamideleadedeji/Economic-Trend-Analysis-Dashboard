# Economic Trend Analysis Dashboard

An interactive dashboard analysing macroeconomic indicators (GDP growth, unemployment, inflation, trade openness) for G7 + BRICS countries (2005–2024) using World Bank data.

**[View the Tableau Public Dashboard](https://public.tableau.com/app/profile/bamidele.adedeji/viz/GlobalEconomicTrendsDashboard)**

## Project Overview
- **Objective:** Identify relationships between key economic indicators and translate them into investment insights.
- **Data source:** World Bank World Development Indicators.
- **Tools:** Python (Pandas, Seaborn, Statsmodels), Tableau Public.

## Key Findings
- **Okun’s Law confirmed:** GDP growth and unemployment are negatively correlated (-0.45).
- **Flattening Phillips Curve:** Inflation shows near‑zero correlation with unemployment.
- **Trade openness:** Stagnant in G7, rising in BRICS – suggesting divergent growth drivers.
- **Regression model:** Inflation = 2.1 + 0.3×GDP_growth – 0.5×Unemployment + 0.1×Trade_Openness (R² = 0.42).

## Repository Structure
economic-trend-dashboard/
├── README.md
├── requirements.txt
├── notebooks/
│ └── analysis.ipynb # ETL + statistical analysis
├── data/
│ └── master_economics.csv # Cleaned dataset
├── dashboard/
│ └── Economic_Trend_Dashboard.twbx # Tableau workbook
└── memo/
└── Investment_Implications.pdf # Final report


## How to Run
1. Clone this repository.
2. Install dependencies: `pip install -r requirements.txt`
3. Open `notebooks/analysis.ipynb` in Jupyter to see the full analysis.

## Dashboard Features
- Interactive line charts with dual axes.
- Correlation heatmap (pre‑computed).
- Recession flag filter (`Unemployment > 8.5% and GDP growth < 2%`).
- Regression coefficients displayed as a table.

## Contact
Created by Bamidele Adedeji  https://www.linkedin.com/in/adedeji-bamidele-88a159263/
