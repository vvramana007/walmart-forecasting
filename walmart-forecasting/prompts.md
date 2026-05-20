# Prompt Log

## Prompt 1
Help me structure a time-series forecasting project comparing retail sales against Walmart revenue.

## Prompt 2
Explain how to create a seasonal naive baseline for quarterly revenue forecasting.

## Prompt 3
How should I perform proper train/test splitting for time-series forecasting?

## Prompt 4
Explain look-ahead bias in simple terms and how to avoid it.

## Prompt 5
Help me compare forecasting performance using MAPE and RMSE.

## Prompt 6
Help me create clean visualization charts for actual vs predicted revenue.

---

# Reflection

The LLM assistant was useful for structuring the workflow, generating starter code, and explaining forecasting concepts. However, some generated suggestions initially used standard train/test splits that were inappropriate for time-series forecasting. I corrected this by using chronological train/test separation and lagged features to avoid look-ahead bias.

I verified outputs by checking:
- date alignment,
- feature lagging,
- train/test separation,
- forecasting metrics,
- and chart consistency.