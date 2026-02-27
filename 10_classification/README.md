# Classification

Notebooks covering supervised classification methods in R — algorithms that predict which category a new observation belongs to based on labeled training data.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `decision_trees.ipynb` | Decision tree classification with `rpart`; pruning and visualization |
| `random_forest.ipynb` | Random forest with `ranger`; variable importance and out-of-bag error |
| `gradient_boosting.ipynb` | XGBoost for classification; tuning, feature importance, and SHAP values; LightGBM as a faster alternative for large datasets |
| `logistic_regression_classification_R.ipynb` | Covers the full arc from standard glm() to regularised logistic regression via glmnet (ridge, LASSO, elastic net with coefficient path visualisation), plus threshold optimisation using Youden's J and max-F1 |
| `model_evaluation.ipynb` | Confusion matrix, AUC-ROC, F1 score, precision-recall curves, and calibration curves |
| `imbalanced_data.ipynb` | Handling class imbalance with SMOTE, ROSE, and cost-sensitive learning |
| `shap_explainability.ipynb` | SHAP values for model interpretability with `shapviz` |
| `gradient_boosting_R.ipynb` | Covers both XGBoost and LightGBM in a single notebook with a side-by-side comparison of the feature importance rankings. The comparison table at the top makes the key differences (leaf-wise vs level-wise, 'num_leaves' vs 'max_depth', native categorical support) concrete before any code runs |
| `ssvm_classification_R.ipynb` | the sigest() function for automatic sigma estimation gets prominent billing since it's the most commonly skipped step. The 2D grid tuning (C × sigma jointly) and the decision boundary visualisation are the two things that make SVMs actually teachable |

---

## Dependencies

```r
install.packages(c("tidyverse", "rpart", "rpart.plot", "ranger", "xgboost",
                   "lightgbm", "caret", "pROC", "ROSE", "themis", "shapviz"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
