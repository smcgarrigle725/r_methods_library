# r_methods_library

A documented reference library of statistical methods implemented in R. Each section contains working code skeletons with explanations of when and why to use each method — written for an audience familiar with data science but not necessarily with R or ecology.

Code is organized by analysis type. Every file is self-contained: load the libraries, read the comments, run the code.

---

## Structure

```
r_methods_library/
│
├── 01_basic_inference/
│   ├── README.md
│   ├── t_tests.R
│   ├── anova.R
│   └── nonparametric_equivalents.R
│
├── 02_regression/
│   ├── README.md
│   ├── linear_regression.R
│   ├── logistic_regression.R
│   ├── regularized_regression.R        # ridge, lasso, elastic net
│   └── glm_count_data.R                # Poisson, negative binomial
│
├── 03_mixed_effects_models/
│   ├── README.md
│   ├── lmm_basics.R                    # lme4
│   └── glmm_basics.R                   # glmmTMB
│
├── 04_gams/
│   ├── README.md
│   ├── gam_basics.R                    # mgcv
│   └── gam_diagnostics.R               # gratia
│
├── 05_multivariate/
│   ├── README.md
│   ├── pca.R
│   ├── nmds.R
│   ├── clustering.R                    # k-means, hierarchical
│   └── permanova.R                     # vegan
│
├── 06_nonparametric/
│   ├── README.md
│   ├── rank_tests.R                    # Mann-Whitney, Kruskal-Wallis
│   └── permutation_tests.R
│
├── 07_time_series/
│   ├── README.md
│   ├── decomposition.R
│   └── arima_basics.R
│
├── 08_bayesian/
│   ├── README.md
│   └── nimble_basics.R
│
└── 09_model_diagnostics/
    ├── README.md
    ├── dharma_residuals.R
    └── model_selection_aic.R
```

---

## Key Packages

| Category | Packages |
|---|---|
| Data manipulation | `tidyverse`, `dplyr` |
| Visualization | `ggplot2`, `ggpubr` |
| Mixed models | `lme4`, `glmmTMB` |
| GAMs | `mgcv`, `gratia` |
| Multivariate | `vegan`, `ade4`, `FactoMineR` |
| Bayesian | `NIMBLE` |
| Model diagnostics | `DHARMa`, `performance` |
| Model selection | `AICcmodavg`, `MuMIn` |
| Nonparametric | `coin`, `nortest` |

---

## Usage

Each `.R` file is structured as follows:

```r
# ── METHOD NAME ──────────────────────────────────────────────
# When to use: ...
# Assumptions: ...
# Industry applications: ...
#
# ── SETUP ────────────────────────────────────────────────────
library(...)

# ── EXAMPLE DATA ─────────────────────────────────────────────
# ...

# ── ANALYSIS ─────────────────────────────────────────────────
# ...

# ── INTERPRETATION ───────────────────────────────────────────
# ...
```

---

*Part of a broader portfolio. See also:
[ecological_data_science](https://github.com/samantha-mcgarrigle/ecological_data_science) ·
[python_methods_library](https://github.com/samantha-mcgarrigle/python_methods_library) ·
[databases](https://github.com/samantha-mcgarrigle/databases)*
