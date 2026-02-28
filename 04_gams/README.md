# 04 · Generalised Additive Models (GAMs)

Flexible regression with smooth, non-linear terms. GAMs extend GLMs by replacing linear predictors with penalised splines — capturing curvature without specifying its form in advance.

| Notebook | Description |
|---|---|
| `gam_basics_R.ipynb` | Smooth terms, basis functions, and GCV penalty selection; `mgcv::gam` |
| `gam_distributions_R.ipynb` | GAMs for Poisson, binomial, gamma, and Tweedie responses |
| `gam_interactions_R.ipynb` | Tensor product smooths; 2D surfaces; factor-smooth interactions |
| `gamm_R.ipynb` | GAMs with random effects (GAMMs); `gamm4` |
| `gam_prediction_R.ipynb` | Prediction, confidence bands, and marginal effects from fitted GAMs |
| `gam_model_checking_R.ipynb` | `gam.check()`, concurvity, basis dimension adequacy, residual diagnostics |

**Key packages:** `mgcv`, `gamm4`, `gratia`, `ggplot2`

---

## Dependencies

```r
install.packages(c("mgcv", "gratia", "tidyverse", "ggplot2", "performance"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
