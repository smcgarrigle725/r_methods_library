# Generalized Additive Models (GAMs)

Notebooks covering GAMs in R using `mgcv`. GAMs extend generalized linear models by allowing predictor-response relationships to be modeled as flexible smooth functions rather than straight lines — making them well-suited to ecological gradients, nonlinear temporal trends, and complex spatial patterns.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `gam_basics.ipynb` | GAM fundamentals: smooth terms, basis functions, and fitting with `mgcv` |
| `gam_families.ipynb` | GAMs with different response distributions: Gaussian, Poisson, binomial, negative binomial, Tweedie |
| `gam_interactions.ipynb` | Tensor product smooths for interactions between continuous predictors |
| `gam_diagnostics.ipynb` | Model checking with `gratia`: residuals, basis dimension, concurvity |
| `gam_visualization.ipynb` | Plotting smooth terms, partial effects, and predictions with `gratia` and `ggplot2` |
| `gam_vs_glm.ipynb` | When to use a GAM vs. a GLM; AIC comparison and interpretability trade-offs |

---

## Dependencies

```r
install.packages(c("mgcv", "gratia", "tidyverse", "ggplot2", "performance"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
