# Regression

Notebooks covering regression methods in R, from simple linear models through generalized linear models for non-normal response variables. Includes assumption testing, diagnostics, and model selection.

All notebooks use built-in R datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `linear_regression.ipynb` | Simple and multiple linear regression, diagnostics, and interpretation |
| `logistic_regression.ipynb` | Binary logistic regression for presence/absence and binary outcome data |
| `multinomial_regression.ipynb` | Multinomial logistic regression for unordered categorical outcomes |
| `ordinal_regression.ipynb` | Ordinal logistic regression for ordered categorical outcomes |
| `glm_count_data.ipynb` | Poisson and negative binomial regression for count data; zero-inflated models |
| `regularized_regression.ipynb` | Ridge, lasso, and elastic net regression for high-dimensional data |
| `regression_diagnostics.ipynb` | Residual analysis, leverage, Cook's distance, VIF, and model fit |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "car", "MASS", "glmmTMB", "pscl",
                   "glmnet", "performance", "effectsize", "broom"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
