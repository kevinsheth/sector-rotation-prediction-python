# Sector Rotation Prediction with Python
## Overview
This project develops a predictive model for sector rotation using high-frequency price data condensed into 30-minute bars to forecast the highest returning sector in the next interval. The sectors are defined by averaging the returns of DJIA stocks within each sector.

## Target
The model aims to predict one out of five sectors that will yield the highest return in the upcoming 30-minute interval.

## Data Transformation
Data is transformed from high-frequency price data to 30-minute bars, then to returns.

## Alternate Data
The project also considers alternate data such as GDP, Jobs, and SPDR ETF Daily Returns as part of the features (X).

## Challenges
The project addresses challenges such as insufficient granularity of external data and potential data leakage.

## Models Used
Random Forest
LSTM
XGBoost

## Current Status
The current models show poor performance (F1/AUC scores), with results not significantly better than chance. Future improvements may include careful data shifting and inclusion of alternate data to enhance predictions.

## Notes
Data leakage is a concern; care is taken to not pair future X data with the wrong Y.
Predictions are shifted accordingly to ensure we are forecasting a future winning sector (Y).
## Contribution
This project is part of a group effort, and contributions are welcome to improve the model's predictive capabilities.
