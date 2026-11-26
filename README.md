# IPL Match Performance & Strategic Analysis (2008–2019)

End-to-end data cleaning, validation, and exploratory data analysis (EDA) of **756 IPL matches** across **12 seasons (2008–2019)** using **Python, Pandas, NumPy, Matplotlib, Seaborn, and Plotly**.

## Data Cleaning & Integrity
- Standardized **41 raw venue names into 33 stadiums** and resolved city naming inconsistencies.
- Imputed **7 missing `city` values** (`"Dubai"`) and verified record integrity across all **756 matches**.
- Consolidated **15 franchise variants into 13 teams**, sanitized **55 umpire names**, and fixed truncated player names.

## Key Analytical Findings
- **Toss-to-Match Conversion:** Across **752 decided matches** (excluding 4 *No Result* games), winning the toss converted into a match win **52.26%** of the time (`393/752`).
- **Toss Decision Impact:** Choosing to **field first** produced a **56.30%** win rate compared to **45.89%** when **batting first**.
- **Edge Cases:** Isolated Duckworth-Lewis (`dl_applied == 1`) matches and tied / Super Over games (`result == 'tie'`) so standard win metrics stay accurate.
