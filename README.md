# EPL Team Performance Analysis (2023-24 and 2024-25)

## Project Overview
This project analyzes English Premier League match data across two seasons (2023-24 and 2024-25) to evaluate team performance from a data analyst perspective.

The notebook focuses on:
- data cleaning and validation
- feature engineering for football metrics
- home/away/overall team summaries
- visualization of performance and rate metrics
- final insights that answer practical football questions

## Dataset Scope
- League: English Premier League (EPL)
- Seasons: 2023-24 and 2024-25
- Rows: 760 matches
- Team entities in combined sample: 23 teams
- Core columns used:
  - `Date`
  - `HomeTeam`
  - `AwayTeam`
  - `FTHG`
  - `FTAG`
  - `FTR`

## Tools and Libraries
- Python
- pandas
- matplotlib
- Jupyter Notebook

## Questions Answered
1. Which teams had the best home record?
2. Which teams had the worst away record?
3. Which teams scored the most goals per match?
4. Which teams conceded the most goals per match?
5. Which teams had the highest clean sheet rate?
6. Which teams failed to score most often?
7. Which teams had the highest BTTS rate?
8. Which teams had the highest over 2.5 rate?
9. What did each team's recent form look like?
10. Which teams were stronger at home than away?

## Method Summary
1. Load EPL CSV files and keep core analysis columns.
2. Run quality checks (nulls, duplicates, label validity).
3. Standardize schema and data types.
4. Create derived flags and metrics:
   - `btts_flag`
   - `over_2_5_flag`
   - result flags (`home_win_flag`, `draw_flag`, `away_win_flag`)
   - clean sheet and failed-to-score flags
5. Build `home_summary`, `away_summary`, and `overall_summary`.
6. Compute rate metrics:
   - goals scored/conceded per match
   - BTTS rate
   - over 2.5 rate
   - clean sheet rate
   - failed-to-score rate
7. Visualize rankings and produce final insights.

## Key Findings
- Best home record: **Liverpool** with **94 home points**.
- Worst away record: **Southampton** with **6 away points**.
- Most goals scored per match: **Liverpool** (**2.26**).
- Most goals conceded per match: **Sheffield United** (**2.74**).
- Highest clean sheet rate: **Arsenal** (**40.8%**).
- Highest failed-to-score rate: **Leicester** (**44.7%**).
- Highest BTTS rate: **Luton** (**81.6%**).
- Highest over 2.5 rate: **Luton** (**71.1%**).
- Best recent form (last 5 matches): **Brighton** (**13 points**, form `WDWWW`).
- Strongest home-vs-away gap: **Newcastle** (**+30 points** home minus away).

## Visual Outputs Included
- Top teams by overall points
- Goals scored/conceded per match rankings
- BTTS and over 2.5 rate rankings
- Clean sheet and failed-to-score rate rankings
- Home-vs-away points gap rankings


```

## Limitations
- Only two seasons are analyzed.
- No advanced context features (xG, injuries, lineups, schedule strength).
- Team-level aggregation may hide opponent-level variation.

