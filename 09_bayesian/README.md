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
| `prior_sensitivity_R.ipynb` | Core demonstration fits the same model across four prior widths (tight/moderate/wide/vague) on both a large and small dataset simultaneously, then visualises the posterior densities overlaid |
| `bayesian_workflow_R.ipynb` | Deliberately engineered to fail on the first model (Poisson) so the PPC failure is concrete and instructive rather than hypothetical. The variance/mean test statistic is the specific PPC that catches the overdispersion, which then motivates the switch to Negative Binomial. The notebook ends with a 10-point checklist formatted as an actual checklist that can live in the folder as a reference card. The workflow loops — that's the main point the pitfalls section reinforces |

---

## Dependencies

```r
install.packages(c("nimble", "coda", "loo", "tidyverse", "ggplot2", "bayesplot"))
```

> **Note:** `NIMBLE` requires a C++ compiler. On Windows, install Rtools first. On macOS, install Xcode command line tools.

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
