# Valorant Competitive Analysis

## Objective
- Analyze player performance across maps
- Identify patterns in key performance metrics
- Handle missing and inconsistent real-world data

## Dataset
- Source: [VLR.gg (scraped / collected)](https://www.kaggle.com/datasets/ryanluong1/valorant-champion-tour-2021-2023-data)
- Data includes player statistics per match
- Missing values present in some matches

## Tools
- Python
- pandas
- numpy
- matplotlib / seaborn
- scikit-learn (if applicable)

## Key Findings
- Certain maps show higher average ACS across all players
- Player ratings vary significantly depending on map choice
- Missing values required careful preprocessing

### Opponent-based loss patterns (advanced analysis)

![Maps lost by opponent](https://github.com/user-attachments/assets/890e405a-8719-4454-af3a-da45de6aa882)

This visualization compares map losses by opponent for high-winrate teams.
It highlights potential counter-play styles and matchup dependencies,
and serves as a deeper exploratory analysis rather than a headline result.

**Key insights:**
- Certain opponents systematically dominate specific map pools.
- Loss distribution suggests preparation gaps rather than random variance.
- This pattern could be used to adjust veto strategies or training focus.

## Future Work
- Include team-based analysis
- Add predictive modeling
- Expand dataset to multiple tournaments

