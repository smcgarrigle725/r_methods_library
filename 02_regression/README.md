# 02 · Regression

Linear and generalised linear models — from simple OLS to count and binary outcomes. Emphasis on correct interpretation, assumption checking, and reporting effect sizes alongside p-values.

| Notebook | Description |
|---|---|
| `simple_linear_regression_R.ipynb` | OLS, R², residual diagnostics, and prediction intervals |
| `multiple_regression_R.ipynb` | Multiple predictors, partial effects, model building, standardised coefficients |
| `logistic_regression_R.ipynb` | Binary outcomes; odds ratios, predicted probabilities, ROC/AUC |
| `poisson_regression_R.ipynb` | Count outcomes; offsets, rate ratios, overdispersion checks |
| `negative_binomial_R.ipynb` | Overdispersed counts; NB vs. Poisson model comparison |
| `beta_regression_R.ipynb` | Proportions and rates bounded (0,1); `betareg` package |
| `ordinal_regression_R.ipynb` | Ordered categorical outcomes; proportional odds model; `MASS::polr` |
| `ancova.ipynb` | ANCOVA as regression with continuous covariate + factor; homogeneity of slopes; adjusted means; when ANCOVA vs factorial ANOVA |
| `model2_regression.ipynb` | Model II regression (major axis, standardised major axis / RMA); when X is also measured with error; morphometrics and allometry |
| `weighted_least_squares.ipynb` | Weighted least squares for heteroscedastic data; known-variance weights; survey weights |
| `log_linear_models.ipynb` | Log-linear models for multi-way contingency tables; model selection beyond chi-square; 3-way tables |
| `smoothing.ipynb` | LOESS/LOWESS, regression splines, and kernel smoothing as standalone tools; distinct from GAMs |

**Key packages:** `stats`, `MASS`, `betareg`, `pROC`, `broom`, `smatr`, `VGAM`, `lmtest`

---
## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "car", "MASS", "glmmTMB", "pscl",
                   "glmnet", "performance", "effectsize", "broom"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
