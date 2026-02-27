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
| `nested_cv.ipynb` | nested cross-validation for simultaneous hyperparameter tuning and unbiased performance estimation; the single most commonly violated principle in applied ML evaluation. Without nesting, models tuned using the outer CV folds produce optimistically biased error estimates. Distinct enough from 'kfold_cv.ipynb' to warrant its own notebook. |
| `bootstrap_resampling.ipynb` | bootstrap for estimating model uncertainty and performance metric confidence intervals; the .632 bootstrap for small samples is essential for ecological and clinical work where n is rarely large. |
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
