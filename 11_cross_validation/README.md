# Cross-Validation & Model Selection

Notebooks covering strategies for evaluating model generalizability and selecting among competing models in R. Proper cross-validation is essential for avoiding overfitting and producing honest estimates of predictive performance.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `train_test_split.ipynb` | Train/validation/test split discipline; data leakage and how to prevent it |
| `kfold_cv.ipynb` | k-fold and stratified k-fold cross-validation with `caret` and `tidymodels` |
| `loocv.ipynb` | Leave-one-out cross-validation; when to use it and computational trade-offs |
| `ts_cv.ipynb` | Time-series-aware cross-validation to preserve temporal order and prevent leakage |
| `hyperparameter_tuning.ipynb` | Grid search and random search for hyperparameter optimization |
| `aic_model_selection.ipynb` | AIC/AICc-based model selection for statistical models; multi-model inference |

---

## Dependencies

```r
install.packages(c("tidyverse", "caret", "tidymodels", "rsample",
                   "AICcmodavg", "MuMIn", "yardstick"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
