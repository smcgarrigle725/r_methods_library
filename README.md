# r_methods_library

A documented reference library of statistical methods implemented in R. Each notebook contains working code with explanations of when and why to use each method, inline assumptions testing, interpretation guidance, and applications across ecology, healthcare, finance, and insurance.

Notebooks are self-contained — built-in or simulated datasets only, no external downloads required.

---

## Structure

| Folder | Contents |
|---|---|
| `01_basic_inference/` | t-tests, ANOVA, chi-square, Fisher's exact, confidence intervals, effect sizes |
| `02_regression/` | Linear, logistic, multinomial, ordinal, GLMs for count data, regularized regression |
| `03_mixed_effects_models/` | LMMs, GLMMs, random effects structure, diagnostics, model selection |
| `04_gams/` | GAM basics, families, interactions, diagnostics, visualization |
| `05_multivariate/` | PCA, nMDS, PERMANOVA, dbRDA, ANOSIM, Mantel test, biplots |
| `06_nonparametric/` | Mann-Whitney, Wilcoxon, Kruskal-Wallis, Spearman, permutation tests, normality tests |
| `07_time_series/` | Decomposition, ARIMA, SARIMA, Prophet, exponential smoothing, TS cross-validation |
| `08_survival_analysis/` | Kaplan-Meier, Cox proportional hazards, AFT models, survival visualization |
| `09_bayesian/` | Bayesian inference with NIMBLE, hierarchical models, MCMC diagnostics, WAIC |
| `10_classification/` | Decision trees, random forest, XGBoost, LightGBM, model evaluation, SHAP |
| `11_cross_validation/` | Train/test split, k-fold CV, LOOCV, time series CV, hyperparameter tuning |
| `12_clustering/` | k-means, hierarchical, DBSCAN, Gaussian mixture models, cluster validation |
| `13_dimensionality_reduction/` | PCA, factor analysis, t-SNE, UMAP, correspondence analysis |
| `14_model_diagnostics/` | Residuals, DHARMa, VIF, Cook's distance, SHAP, partial dependence, feature importance |
| `15_ab_testing/` | Power analysis, proportion and mean tests, multiple testing, experiment design |

---

## Notebook Structure

Every notebook follows this consistent template:

1. **Overview** — what the method does, when to use it
2. **Applications by Sector** — ecology, healthcare, finance, insurance examples
3. **Assumptions Checklist** — static reference list
4. **Setup** — libraries and reproducibility
5. **Data** — built-in or simulated dataset with description
6. **Assumptions Testing** — inline tests run before the model
7. **Analysis** — main implementation with comments
8. **Interpretation** — how to read the output
9. **Reporting** — standard format for results
10. **Common Pitfalls** — what to watch out for

---

## Setup

### IRkernel (required to run R notebooks in Jupyter)

```r
# Run once in R
install.packages("IRkernel")
IRkernel::installspec()
```

Then launch Jupyter and select **R** as the kernel when creating a new notebook.

### Core dependencies

```r
# Install all packages used across the library
install.packages(c(
  # Data manipulation & visualization
  "tidyverse", "ggplot2", "ggpubr", "broom",
  # Inference & nonparametrics
  "car", "effectsize", "rstatix", "pwr", "coin", "nortest", "dunn.test",
  # Regression & GLMs
  "MASS", "glmnet", "pscl", "performance",
  # Mixed models
  "lme4", "glmmTMB", "DHARMa", "AICcmodavg", "MuMIn", "broom.mixed",
  # GAMs
  "mgcv", "gratia",
  # Multivariate
  "vegan", "ade4", "FactoMineR", "factoextra",
  # Time series
  "forecast", "tseries", "prophet", "lubridate", "zoo",
  # Survival
  "survival", "survminer",
  # Bayesian
  "nimble", "coda", "loo", "bayesplot",
  # Classification & ML
  "rpart", "rpart.plot", "ranger", "xgboost", "lightgbm",
  "caret", "pROC", "ROSE", "themis", "shapviz", "pdp", "vip",
  # Clustering & dimensionality reduction
  "cluster", "dbscan", "mclust", "Rtsne", "umap", "psych",
  # Tidymodels ecosystem
  "tidymodels", "rsample", "yardstick"
))
```

---

*Part of a broader portfolio. See also:
[ecological_data_science](https://github.com/samantha-mcgarrigle/ecological_data_science) ·
[python_methods_library](https://github.com/samantha-mcgarrigle/python_methods_library) ·
[databases](https://github.com/samantha-mcgarrigle/databases) ·
[industry_projects](https://github.com/samantha-mcgarrigle/industry_projects)*
