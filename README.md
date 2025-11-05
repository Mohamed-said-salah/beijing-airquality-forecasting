# Beijing PM2.5 Air Quality Forecasting

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Vz4eT3TREboW0NDMPENxCGTOOpX97TDN?usp=sharing)

End-to-end time-series ML forecasting for **PM2.5** air pollution levels in Beijing (2010–2014).

## Dataset
- Source: [UCI / J. Brownlee Datasets – pollution.csv](https://raw.githubusercontent.com/jbrownlee/Datasets/master/pollution.csv)
- Hourly meteorological and pollution measurements.
- Preprocessing: datetime index, missing value interpolation, scaling.

## Methods
- Lags & rolling window features (1–24h)
- Models: Linear Regression, Random Forest, XGBoost
- Chronological split (no leakage)
- Evaluation: RMSE, MAE, R² vs persistence baseline

## Results
- Best model: LR with Test RMSE = 0.00
- Baseline RMSE = 22.08

## Report
See `reports/Beijing_PM25_Forecasting_Report.pdf` (auto-generated from notebook).
