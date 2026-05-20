# Walmart Revenue Forecasting using FRED Retail Sales

This project evaluates whether monthly U.S. retail-sales data from FRED can predict Walmart quarterly revenue better than a seasonal naive baseline.

## Objective

Test whether retail-sales data provides incremental forecasting power for Walmart revenue prediction.

## Dataset

- FRED Retail Sales (RSXFS)
- Walmart Quarterly Revenue

## Approach

1. Converted monthly retail-sales data into quarterly aggregates
2. Built seasonal naive baseline
3. Engineered lagged retail-sales features
4. Trained linear regression forecasting model
5. Evaluated using:
   - MAPE
   - RMSE
6. Compared out-of-sample forecasting performance

## Key Findings

- Retail-sales data modestly improved forecasting accuracy relative to the baseline.
- Forecast performance weakened during structurally unusual periods such as COVID-19.
- Retail sales should be treated as a supplemental forecasting signal rather than a standalone predictor.

## Tech Stack

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Google Colab

## Project Structure

```text
yipitdata-walmart-forecasting/
├── analysis.ipynb
├── memo.md
├── prompts.md
├── requirements.txt
└── data/
```

## Future Improvements

- Add macroeconomic variables
- Test ARIMA/XGBoost models
- Use retailer-specific subsector data
- Add rolling-window forecasting evaluation

## Author

Venkata Ramana Veeraiahgari