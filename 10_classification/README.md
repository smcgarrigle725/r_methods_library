# 10 · Classification

Supervised learning for categorical outcomes. Covers classical statistical classifiers through ensemble methods, with consistent emphasis on proper evaluation and avoiding common sources of inflated performance estimates.

| Notebook | Description |
|---|---|
| `logistic_classification_R.ipynb` | Logistic regression as a classifier; threshold selection; ROC/AUC |
| `lda_qda_classification_R.ipynb` | Linear and quadratic discriminant analysis; decision boundaries |
| `decision_trees_R.ipynb` | CART; pruning; visualising splits; `rpart` |
| `random_forest_R.ipynb` | Bagging ensemble; OOB error; variable importance; `ranger` |
| `gradient_boosting_R.ipynb` | XGBoost and LightGBM; learning rate, depth, early stopping |
| `svm_R.ipynb` | Support vector machines; kernel trick; hyperparameter tuning |
| `naive_bayes_R.ipynb` | Naive Bayes classifier; Laplace smoothing; text and tabular data |
| `model_evaluation_classification_R.ipynb` | Confusion matrix, precision, recall, F1, ROC, calibration curves |

**Key packages:** `ranger`, `xgboost`, `e1071`, `caret`, `pROC`, `yardstick`

---

## Dependencies

```r
install.packages(c("tidyverse", "rpart", "rpart.plot", "ranger", "xgboost",
                   "lightgbm", "caret", "pROC", "ROSE", "themis", "shapviz"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
