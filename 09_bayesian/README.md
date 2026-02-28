# 09 · Bayesian Methods

Bayesian inference using Stan and related tools. Covers the full workflow from prior specification to posterior diagnostics, with an emphasis on principled uncertainty quantification.

| Notebook | Description |
|---|---|
| `bayes_intro_R.ipynb` | Prior, likelihood, posterior; conjugate models; grid approximation |
| `mcmc_diagnostics_R.ipynb` | Trace plots, R-hat, ESS, divergences; identifying sampling failures |
| `brms_regression_R.ipynb` | Bayesian linear and GLM regression with `brms`; prior predictive checks |
| `hierarchical_models_R.ipynb` | Partial pooling; multilevel Bayesian models; shrinkage |
| `model_comparison_bayes_R.ipynb` | LOO-CV, WAIC, Bayes factors; `loo` package |
| `posterior_predictive_R.ipynb` | Posterior predictive checks; `bayesplot`; calibration |
| `stan_custom_R.ipynb` | Writing custom Stan models; blocks, transformed parameters, generated quantities |

**Key packages:** `brms`, `rstan`, `loo`, `bayesplot`, `posterior`

---

## Dependencies

```r
install.packages(c("nimble", "coda", "loo", "tidyverse", "ggplot2", "bayesplot"))
```

> **Note:** `NIMBLE` requires a C++ compiler. On Windows, install Rtools first. On macOS, install Xcode command line tools.

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
