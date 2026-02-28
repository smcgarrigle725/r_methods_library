# 11 · Cross-Validation and Model Selection

Rigorous model evaluation and selection. The central theme throughout is the strict separation of training, validation, and test data — and the consequences of violating it.

| Notebook | Description |
|---|---|
| `train_test_split_R.ipynb` | Holdout evaluation; stratified splitting; the test set is not for tuning |
| `kfold_cv_R.ipynb` | k-fold CV; stratification; repeated CV for variance reduction |
| `loocv_R.ipynb` | Leave-one-out CV; when it is and isn't appropriate; computational shortcuts |
| `ts_cv_R.ipynb` | Time-series-aware CV; expanding and sliding window; no future leakage |
| `hyperparameter_tuning_R.ipynb` | Grid search, random search, and Bayesian optimisation; tuning inside CV |
| `aic_bic_model_selection_R.ipynb` | AIC, AICc, BIC; multi-model inference; Akaike weights |
| `regularisation_R.ipynb` | Ridge, LASSO, elastic net; `glmnet`; CV for penalty selection |
| `nested_cv_R.ipynb` | Nested CV for simultaneous tuning and unbiased evaluation |
| `bootstrap_resampling_R.ipynb` | Bootstrap CIs for any statistic; .632 bootstrap for small samples |

**Key packages:** `caret`, `tidymodels`, `glmnet`, `rsample`, `yardstick`

---

## Dependencies

```r
install.packages(c("tidyverse", "caret", "tidymodels", "rsample",
                   "AICcmodavg", "MuMIn", "yardstick"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
