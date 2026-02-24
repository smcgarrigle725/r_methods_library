# Classification

Notebooks covering supervised classification methods in R — algorithms that predict which category a new observation belongs to based on labeled training data.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `decision_trees.ipynb` | Decision tree classification with `rpart`; pruning and visualization |
| `random_forest.ipynb` | Random forest with `ranger`; variable importance and out-of-bag error |
| `gradient_boosting_xgboost.ipynb` | XGBoost for classification; tuning, feature importance, and SHAP values |
| `gradient_boosting_lightgbm.ipynb` | LightGBM as a faster alternative for large datasets |
| `model_evaluation.ipynb` | Confusion matrix, AUC-ROC, F1 score, precision-recall curves, and calibration curves |
| `imbalanced_data.ipynb` | Handling class imbalance with SMOTE, ROSE, and cost-sensitive learning |
| `shap_explainability.ipynb` | SHAP values for model interpretability with `shapviz` |

---

## Dependencies

```r
install.packages(c("tidyverse", "rpart", "rpart.plot", "ranger", "xgboost",
                   "lightgbm", "caret", "pROC", "ROSE", "themis", "shapviz"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
