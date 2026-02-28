# 08 · Survival Analysis

Methods for time-to-event data where outcomes may be censored. Applicable to species persistence, time-to-recolonisation, clinical endpoints, and any setting where the event of interest may not be observed for all subjects.

| Notebook | Description |
|---|---|
| `kaplan_meier_R.ipynb` | KM estimator; survival curves; log-rank test; `survfit` |
| `cox_regression_R.ipynb` | Cox proportional hazards model; hazard ratios; Schoenfeld residuals |
| `parametric_survival_R.ipynb` | Weibull, exponential, log-normal AFT models; `survreg` |
| `competing_risks_R.ipynb` | Fine-Gray model; cause-specific hazards; cumulative incidence functions |
| `time_varying_covariates_R.ipynb` | Counting process formulation; time-updated exposures in Cox models |
| `frailty_models_R.ipynb` | Random effects (frailties) for clustered survival data |

**Key packages:** `survival`, `survminer`, `cmprsk`, `frailtypack`

---

## Applications by Sector

| Sector | Example |
|---|---|
| **Ecology** | Time to recolonization of disturbed habitat; survival of transplanted organisms; time to first detection of a species post-restoration |
| **Healthcare** | Patient survival post-diagnosis; time to hospital readmission; time to disease progression |
| **Finance** | Time to loan default; customer churn (time to account closure); time to first transaction |
| **Insurance** | Time to first claim; claims duration modeling; time to policy lapse |

---

## Dependencies

```r
install.packages(c("survival", "survminer", "tidyverse", "ggplot2", "broom"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
