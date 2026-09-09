# NBA MVP Statistical Metric

## Project Overview
This project evaluates whether a  quantitative statistical model can accurately identify the NBA Most Valuable Player (MVP) winner and finalists. This analysis aims to separate subjective media narrative from objective statistical performance.

## Key Results 
  - Top 5 Finalists: the model successfully identified an average of 3.6 out of 5 actual MVP finalists per season.
  - Winner Accuracy: the model correctly predicted the exact MVP winner in 50% of the seasons analyzed.
  - Top 2 Precision: the predicted winner fell within the actual top 2 MVP finalists 90% of the time.

## Methodology 
  - Language: Python
  - Libraries: Pandas, NumPy
  - Data Source: Regular season per-game and advanced tables from Basketball Reference
  - Feature Scaling: Engineered data using Z-scores to standardize core metrics to compare players fairly against the league average

## The Formula
The custom MVP Score utilizes a manually weighted sum or box score and advanced statistics:

MVP Score = 0.30(PTS) + 0.15(AST) + 0.10(TRB) + 0.15(TS%) + 0.20(VORP) + 0.10(DEF)

(DEF is a combined metric of Steals + Blocks, and TS% accounts for scoring volume efficiency)

## Future Enhancements
- Incorporate team win-loss records to account for team success biases.
- Expand dataset back further into NBA history to test the model's performance across different eras.
- Use machine learning techniques to discover optimal weights as opposed to manual weight assignment. 
