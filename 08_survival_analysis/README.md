# Survival Analysis

Notebooks covering time-to-event analysis in R. Survival analysis models the time until an event of interest occurs — and crucially, handles *censored* observations where the event has not yet occurred by the end of the study period.

Originally developed for clinical research, these methods transfer directly to any domain where time-to-event is the outcome of interest.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `kaplan_meier.ipynb` | Kaplan-Meier survival curves: estimation, visualization, and log-rank test |
| `cox_proportional_hazards.ipynb` | Cox PH model: fitting, assumption checking (proportional hazards), and interpretation of hazard ratios |
| `accelerated_failure_time.ipynb` | AFT models as a parametric alternative to Cox regression |
| `survival_visualization.ipynb` | Publication-quality survival curves with confidence intervals using `survminer` |
| `competing_risks.ipynb` | When subjects can fail from multiple causes (invertebrate lost to predation vs. desiccation; patient dies from cancer vs. cardiovascular disease); cumulative incidence functions and Fine-Gray subdistribution hazards. Frequently needed and frequently mishandled with standard KM |
| `time_varying_covariates.ipynb` | covariates that change value during follow-up (treatment dose changes, habitat quality measured at multiple points); extends Cox and fixes a major assumption violation people routinely miss |

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
