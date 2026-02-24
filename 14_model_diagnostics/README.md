# Model Diagnostics & Interpretation

Notebooks covering tools for evaluating whether a model is well-specified, checking that assumptions are met post-fitting, and interpreting what a model has learned. Good diagnostics are what separate a trustworthy analysis from one that merely produces output.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `residual_diagnostics.ipynb` | Residual plots, Q-Q plots, scale-location, and influential observations for linear models |
| `dharma_diagnostics.ipynb` | Simulation-based residual diagnostics for GLMMs and other complex models using `DHARMa` |
| `multicollinearity.ipynb` | Variance inflation factor (VIF), correlation matrices, and strategies for handling collinearity |
| `influential_observations.ipynb` | Cook's distance, leverage, DFFITS, and handling outliers responsibly |
| `shap_values.ipynb` | SHAP values for global and local model interpretation with `shapviz` |
| `partial_dependence.ipynb` | Partial dependence plots and individual conditional expectation (ICE) curves |
| `permutation_importance.ipynb` | Permutation-based feature importance with `vip` |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "DHARMa", "performance",
                   "car", "shapviz", "pdp", "vip", "broom"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
