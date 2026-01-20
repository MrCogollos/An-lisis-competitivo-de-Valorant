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

  ### Model performance (ROC curve)

![Random Forest ROC Curve](https://github.com/user-attachments/assets/7c0b7556-79af-4f88-adf2-783b5f4fa8c2)


The ROC curve evaluates the discriminative ability of the Random Forest model
to predict map-level outcomes. The model achieves a strong ROC-AUC score,
indicating good separation between wins and losses across different thresholds.


  ### Feature importance (Random Forest)

![Top 20 feature importances](https://github.com/user-attachments/assets/10647b52-68a8-44bb-8f88-9448ff362f0b)


This visualization shows the top 20 most important features used by the
Random Forest model to predict map outcomes.

**Key observations:**
- Performance metrics such as Rating, ACS, KAST%, ADR and KD are the strongest
  contributors to map-level win probability.
- Contextual categorical variables (Map, Team, Opponent, Region) also play a
  significant role after one-hot encoding.
- The results align with competitive intuition: consistent round impact and
  efficiency matter more than raw kill counts alone.

This analysis improves model transparency and helps connect statistical results
with in-game performance factors.



## Future Work
- Include team-based analysis
- Add predictive modeling
- Expand dataset to multiple tournaments

