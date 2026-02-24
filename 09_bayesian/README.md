# Bayesian Methods

Notebooks covering Bayesian statistical inference in R using `NIMBLE`. Bayesian methods treat parameters as probability distributions rather than fixed values, allowing explicit incorporation of prior knowledge and full quantification of uncertainty.

All notebooks use simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `bayesian_fundamentals.ipynb` | Prior, likelihood, posterior — the Bayesian workflow; MCMC concepts |
| `bayesian_linear_regression.ipynb` | Bayesian linear regression with `NIMBLE`; comparing to frequentist results |
| `hierarchical_models.ipynb` | Bayesian hierarchical (multilevel) models; partial pooling and shrinkage |
| `mcmc_diagnostics.ipynb` | Trace plots, R-hat, effective sample size, and posterior predictive checks with `coda` |
| `model_comparison_waic.ipynb` | Bayesian model comparison using WAIC and LOO-CV with the `loo` package |

---

## Dependencies

```r
install.packages(c("nimble", "coda", "loo", "tidyverse", "ggplot2", "bayesplot"))
```

> **Note:** `NIMBLE` requires a C++ compiler. On Windows, install Rtools first. On macOS, install Xcode command line tools.

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
