# 07 · Time Series

Analysis and forecasting of temporally ordered data. Covers classical decomposition through state-space models, with emphasis on ecological monitoring and environmental data applications.

| Notebook | Description |
|---|---|
| `ts_basics_R.ipynb` | `ts` objects, plotting, ACF/PACF, stationarity, differencing |
| `decomposition_R.ipynb` | STL, classical, and X11 decomposition; trend/seasonality separation |
| `arima_R.ipynb` | ARIMA modelling; `auto.arima`; model identification and diagnostics |
| `sarima_R.ipynb` | Seasonal ARIMA; handling periodic patterns in ecological time series |
| `exponential_smoothing_R.ipynb` | ETS models; Holt-Winters; forecast::ets |
| `prophet_R.ipynb` | Facebook Prophet for trend + seasonality + changepoints |
| `intervention_analysis_R.ipynb` | Interrupted time series; detecting change after an event |
| `multivariate_ts_R.ipynb` | VAR models; Granger causality; impulse response functions |
| `ts_cross_validation_R.ipynb` | Time-series-aware CV; expanding and sliding window evaluation |
| `garch_R.ipynb` | Volatility modelling; ARCH/GARCH for non-constant variance |

**Key packages:** `forecast`, `tseries`, `prophet`, `vars`, `rugarch`

---

## Dependencies

```r
install.packages(c("tidyverse", "forecast", "tseries", "prophet",
                   "ggplot2", "lubridate", "zoo"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
