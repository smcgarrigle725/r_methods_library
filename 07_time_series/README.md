# Time Series Analysis

Notebooks covering time series decomposition, modeling, and forecasting in R. Time series methods are applicable to ecological monitoring data, patient longitudinal records, financial price series, and insurance claims trends.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `stationarity.ipynb` | ADF/KPSS tests, unit roots, differencing to achieve stationarity |
| `decomposition.ipynb` | Trend, seasonality, and residual decomposition using classical and STL methods |
| `acf_pacf.ipynb` | Autocorrelation and partial autocorrelation functions; identifying AR and MA structure |
| `arima.ipynb` | ARIMA modeling: identification, fitting, diagnostics, and forecasting |
| `sarima.ipynb` | Seasonal ARIMA for data with periodic patterns |
| `exponential_smoothing.ipynb` | Exponential smoothing and Holt-Winters models |
| `prophet_forecasting.ipynb` | Facebook Prophet for flexible trend and seasonality forecasting |
| `intervention_analysis.ipynb` | Detecting and modelling structural breaks, step changes, and pulse events in time series; directly relevant to before/after ecological assessments, policy changes, treatment rollouts |
| `ts_regression.ipynb` | Regression with autocorrelated errors (GLS/ARIMA errors); bridges time series and regression folders and covers a very common applied case |
| `ts_cross_validation.ipynb` | Time-series-aware cross-validation to prevent data leakage |

---

## Dependencies

```r
install.packages(c("tidyverse", "forecast", "tseries", "prophet",
                   "ggplot2", "lubridate", "zoo"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
