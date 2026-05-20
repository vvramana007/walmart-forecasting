# Walmart Revenue Forecasting Memo

## Question

Can FRED retail-sales data predict Walmart quarterly revenue better than a naive baseline?

---

## Short Answer

Yes, the retail-sales model provided modest forecasting improvement over the seasonal naive baseline during normal economic periods. However, the relationship weakened during structurally unusual periods such as COVID-19.

---

## Approach

I compared two approaches:

1. Seasonal naive baseline:
   - Predict current quarter revenue using the same quarter from the previous year.

2. Retail-sales forecasting model:
   - Used lagged retail-sales growth and lagged Walmart growth as predictive features.
   - Evaluated using out-of-sample time-series testing.

Performance was measured using:
- MAPE
- RMSE

---

## Key Findings

- The retail-sales model modestly improved prediction accuracy relative to the seasonal naive baseline.
- Retail sales appeared more useful during stable macroeconomic periods.
- Forecast quality deteriorated during COVID-related disruptions, suggesting the relationship is regime-dependent rather than universally stable.

---

## Risks and Caveats

1. Limited sample size due to quarterly data frequency.
2. COVID created structural breaks in consumer behavior.
3. Retail sales may correlate with Walmart revenue without directly causing it.
4. Forecasting systems must avoid look-ahead bias by using only data available at prediction time.
5. Walmart-specific operational factors are not captured by macro retail-sales data.

---

## Recommendation

Retail sales should be treated as a supplemental forecasting signal rather than a standalone predictor. It can improve forecasts modestly when combined with historical Walmart revenue patterns, but its usefulness depends on economic stability and proper handling of timing assumptions.