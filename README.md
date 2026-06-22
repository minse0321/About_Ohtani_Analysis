# About_Ohtani_Analysis
Shohei Ohtani career batting analysis using MLB Statcast data (pybaseball + SQL + Python + Tableau)
# ⚾ Shohei Ohtani — Career Batting Analysis

## Overview
MLB Statcast data analysis of Shohei Ohtani's career batting performance (2018–2025, Regular Season only).  
Data collected via pybaseball API → SQLite DB → SQL queries → Python visualization → Tableau dashboard.

## ✨Key Insights
> **Ohtani's peak came after joining the Dodgers.**  
> Exit velocity rose from 92.6 mph (2018) to 95.7 mph (2024), and home runs increased from 22 to 55 over his career.  
> His 2021 season (+39 HR vs prior year) marked the biggest single-season jump in his career.

## 🏟️Tech Stack
- **pybaseball** — MLB Statcast API data collection
- **SQLite + SQL** — data storage & querying (SELECT, GROUP BY, CASE WHEN, Subquery, Window Functions)
- **Python** (Pandas, Matplotlib) — EDA & visualization
- **Tableau Public** — interactive dashboard

## SQL Skills Demonstrated
| Skill | Used For |
|---|---|
| `GROUP BY` | Season & pitch type aggregation |
| `CASE WHEN` | Home run counting by pitch type |
| `SUBSTR` | Extracting year from game_date |
| `Subquery` | Filtering seasons above career average |
| `RANK() OVER` | Career HR ranking by season |
| `LAG() OVER` | YoY home run change |

## Project Structure
├── Ohtani_Analysis.ipynb      # Full analysis notebook

├── ohtani_season_stats.csv    # Season-level stats (2018-2025)

└── ohtani_pitch_stats.csv     # Pitch type breakdown


## Dashboard
🔗 [View on Tableau Public](여기에_태블로_링크_나중에_추가)

## Data Note
- Source: MLB Baseball Savant via pybaseball
- Filtered to Regular Season only (`game_type = 'R'`)
- Postseason data excluded to match official MLB stats
