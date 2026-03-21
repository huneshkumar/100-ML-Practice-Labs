# Project 14 — General Election 1970 to 2024 EDA

## Problem Statement

Explore historical general election data (1970–2024) at the National Assembly (NA) constituency level to understand voting patterns, party performance, turnout, regional variation (province, district, division), and vote shares over time.

## Dataset

- **Source:** `../datasets/general_election_1970to2024.csv`
- **Key columns (examples):** Year, Constituency, NA, Province, District, Division, Party, Candidate Name, regional groupings (Regions 11/12, Regions 5, Zones 20), Registered Voters, Rejected Votes, Six Parties, Turnout N, Votes

## Analysis Performed

- Load and inspect data; shape, info, missing values.
- Analyze elections by year, province, party, and constituency.
- Numerical summaries for votes, turnout, and registered voters where available.
- Visualizations (trends over time, party comparisons, regional breakdowns).
- Document insights on electoral trends and data quality notes.

## Key Insights (Summary)

- How party vote totals and seat-related patterns evolve across election years.
- Regional differences (e.g. by province or zone).
- Turnout and rejected-vote patterns where columns are complete.

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
