# r_methods_library

A reference library of statistical methods implemented in R, organised by topic. Each notebook covers one method or closely related group of methods: a conceptual overview, worked R code on simulated ecological data, and a dedicated pitfalls section documenting the most common misapplications.

## Structure

| Folder | Topic | Notebooks |
|---|---|---|
| `01_basic_inference` | t-tests, ANOVA, chi-squared, confidence intervals | 4 |
| `02_regression` | OLS through ordinal regression; GLMs | 7 |
| `03_mixed_effects_models` | Random intercepts, slopes, GLMMs, model selection | 5 |
| `04_gams` | Penalised splines; GAMs and GAMMs | 6 |
| `05_multivariate` | MANOVA, discriminant analysis, canonical correlation | 10 |
| `06_nonparametric` | Rank-based tests; permutation tests | 5 |
| `07_time_series` | ARIMA, ETS, VAR, intervention analysis, GARCH | 10 |
| `08_survival_analysis` | Kaplan-Meier, Cox regression, competing risks | 6 |
| `09_bayesian_methods` | Stan/brms; hierarchical models; LOO-CV | 7 |
| `10_classification` | Random forest, XGBoost, SVM, model evaluation | 8 |
| `11_cross_validation_model_selection` | CV variants, regularisation, nested CV, bootstrap | 9 |
| `12_clustering` | k-means, hierarchical, DBSCAN, GMMs, validation, profiling | 7 |
| `13_dimensionality_reduction` | PCA, FA, t-SNE, UMAP, CA, nMDS, sparse methods | 7 |
| `14_model_diagnostics_interpretation` | Residuals, DHARMa, SHAP, ALE, permutation importance | 10 |
| `15_ab_testing_experimental_design` | Power, A/B tests, sequential testing, factorial designs | 8 |
| **Total** | | **109** |

## Design principles

**One concept per notebook.** Each notebook has a narrow scope — `kfold_cv_R.ipynb` covers k-fold CV only, not all of cross-validation. This makes individual notebooks easier to use as references.

**Simulated ecological data throughout.** All examples use simulated water quality, species richness, or site-level data. Simulated data means the ground truth is known, which makes it possible to demonstrate what correct and incorrect analyses actually produce.

**Pitfalls section in every notebook.** The final section of each notebook documents five common mistakes for that method — not as a checklist but as worked explanations of *why* each mistake matters and what it produces.

**Methods build on each other.** The folder order is intentional: regression before mixed models, GLMs before GLMMs, basic clustering before validation. Where a notebook depends on concepts from another, it is noted in the overview.

## Usage

Each notebook is self-contained: run from top to bottom in a fresh R kernel. All data are simulated within the notebook using `set.seed()` for reproducibility.

Required packages are listed at the top of each notebook's setup cell and in each folder's `README.md`.

## Author

Samantha McGarrigle · [github.com/samantha-mcgarrigle](https://github.com/samantha-mcgarrigle)
