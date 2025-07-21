# Fantasy Team Simulation using Player Selection Probabilities

_A Data Science Internship Assignment_

---

## Overview

This repository contains a Python-based solution for simulating approximately **20,000 unique fantasy cricket teams** using player selection probabilities. The solution ensures the frequency of each player's selection matches their `perc_selection` value as closely as possible, with all team and role constraints satisfied.

---

## Problem Statement

- **Objective:**  
  Build 20,000 unique fantasy teams (11 players per team) with:
  - At least **one player from each role**: Batsman, Bowler, WK (Wicket Keeper), Allrounder
  - Each team unique (no duplicate combinations)
  - Frequency of each player’s selection across all teams should be close to `perc_selection * 20000`
- **Data Source:**  
  `player_data_sample.csv` — Contains player details & selection probabilities

---

## Key Features

- **Constraint-Driven Team Generation:** Each team strictly meets all required composition rules
- **Probability Matching:** Optimizes player appearance to align with provided selection probabilities
- **Automatic Evaluation:** Comprehensive printout and accuracy summary highlighting selection alignment
- **Exported Outputs:** 
  - All generated teams (`team_df.csv`)
  - Selection accuracy per player (`accuracy_summary.csv`)
- **Bonus:** (Optional) Interactive selection distribution visualization via Plotly (`selection_distribution.html`)

---

## Files

| File Name                                                             | Description                                                           |
|-----------------------------------------------------------------------|-----------------------------------------------------------------------|
| Fantasy_Team_Simulation_using_Player_Selection_Probabilities.ipynb     | Main Jupyter Notebook with full logic and outputs                     |
| player_data_sample.csv                                                | Source CSV with player selection probabilities                        |
| team_df.csv                                                           | Generated teams with player details & team assignment                 |
| accuracy_summary.csv                                                  | Player-level actual vs. expected selection accuracy                   |
| selection_distribution.html                                            | *(Optional)* Interactive chart with target vs. actual selection rates |

---

## How to Use

1. **Clone/Download** this repository.
2. Place your `player_data_sample.csv` in the repo directory.
3. Open and **run the notebook** (`.ipynb`), which will:
   - Build all required teams
   - Calculate and print selection accuracy
4. **Inspect outputs:**  
   - Review `team_df.csv` for all teams  
   - Check `accuracy_summary.csv` for player-level accuracy
   - *(Optional)* Open `selection_distribution.html` for a visual comparison
5. **Review evaluation output:** Generous logging and pass/fail printouts are included.

---

## Example Evaluation Output
