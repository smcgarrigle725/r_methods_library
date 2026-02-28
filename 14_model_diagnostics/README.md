# 14 · Model Diagnostics and Interpretation

Two complementary concerns in one folder: **diagnostics** (is the model valid?) and **interpretation** (what does the model say?). Diagnostics notebooks should be consulted before interpreting any model; interpretation notebooks are most useful after a well-specified model has passed diagnostics.

## Diagnostics

| Notebook | Description |
|---|---|
| `residual_diagnostics_R.ipynb` | The four standard plots; formal tests (Shapiro-Wilk, Breusch-Pagan, Durbin-Watson); robust SEs |
| `dharma_diagnostics_R.ipynb` | Simulation-based residuals for GLMMs and any complex model; dispersion, zero-inflation, outlier tests |
| `multicollinearity_R.ipynb` | VIF, condition number, correlation matrices; remedies including ridge regression and PCA regression |
| `influential_observations_R.ipynb` | Cook's distance, leverage, DFFITS, DFBETAS; the decision framework for what to do with flagged points |
| `overdispersion_R.ipynb` | Detecting overdispersion in count and binary models; quasi-Poisson, negative binomial, zero-inflated models |
| `model_comparison_R.ipynb` | LRT for nested models; AIC/AICc/BIC comparison; REML vs. ML; parametric bootstrap for random effects |

## Interpretation

| Notebook | Description |
|---|---|
| `shap_values_R.ipynb` | Tree SHAP via `shapviz`; beeswarm, dependence, and waterfall plots; global and local interpretation |
| `partial_dependence_R.ipynb` | PDPs and ICE curves; 2D interaction surfaces; when PDPs mislead with correlated features |
| `accumulated_local_effects_R.ipynb` | ALE plots as bias-corrected alternative to PDPs; 2D ALE for interactions; `iml` package |
| `permutation_importance_R.ipynb` | Model-agnostic permutation importance on test data; uncertainty via repeated permutations; `vip` |

**Key packages:** `DHARMa`, `car`, `lmtest`, `sandwich`, `shapviz`, `pdp`, `iml`, `vip`, `xgboost`

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "DHARMa", "performance",
                   "car", "shapviz", "pdp", "vip", "broom"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
