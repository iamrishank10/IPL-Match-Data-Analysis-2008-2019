# IPL Match Performance & Strategic Analysis (2008–2019)

End-to-end data cleaning, validation, and exploratory data analysis (EDA) of **756 IPL matches** across **12 seasons (2008–2019)** and **18 columns**, built with **Python, Pandas, NumPy, Matplotlib, Seaborn, and Plotly**.

## Project Overview
This project turns a raw, inconsistent IPL match dataset into a verified analytical dataset (`756` records) and explores match outcomes across seasons, teams, venues, toss decisions, winning margins, and special match rules (D/L method and tied / Super Over games).

## Data Cleaning & Integrity Pipeline
- **Venue & City Standardization:** Consolidated **41 raw venue entries into 33 standardized stadiums** and resolved city naming inconsistencies.
- **Missing Value Imputation:** Imputed **7 missing `city` values** (`"Dubai"`) and verified overall dataset integrity across all **756 matches** and **18 columns**.
- **Franchise & Name Sanitization:** Consolidated **15 team name variants into 13 teams**, sanitized **55 umpire names**, and fixed truncated player names so team, toss, winner, and player aggregations stay consistent.
- **Clean Dataset Export:** Saved the verified DataFrame after analysis into `IPL_Matches_Cleaned.csv` and `IPL_Matches_Cleaned.xlsx`.

## Key Analytical Findings
- **Toss-to-Match Conversion:** Across **752 decided matches** (excluding 4 *No Result* games), winning the toss converted into a match win **52.26%** of the time (`393/752`).
- **Toss Decision Advantage:** Choosing to **field first** produced a **56.30%** win rate compared to **45.89%** when **batting first**.
- **Edge Cases (`D/L` & Ties):** Isolated Duckworth-Lewis (`dl_applied == 1`) matches and tied / Super Over games (`result == 'tie'`) so standard win-margin distributions and match-win comparisons remain accurate.
- **Exploratory Visualizations:** Generated multi-library charts covering season-wise match volume, team win counts and win percentages, toss decisions, victory margins, and standout performers.

## Repository Structure
- `IPL_Match_Performance_Analysis.ipynb` — Complete end-to-end cleaning, analysis, and visualization notebook
- `IPL_Matches_Cleaned.csv` — Cleaned IPL matches dataset (CSV format)
- `IPL_Matches_Cleaned.xlsx` — Cleaned IPL matches dataset (Excel format)
- `IPL_Matches_Data Analysis.xlsx` — Original raw dataset
- `README.md` — Project documentation and summary

## How to Run
1. Clone or download this repository.
2. Open `IPL_Match_Performance_Analysis.ipynb` in Google Colab or Jupyter Notebook.
3. Run all cells sequentially from top to bottom.
