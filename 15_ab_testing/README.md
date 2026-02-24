# A/B Testing & Experimental Design

Notebooks covering the statistical foundations of controlled experiments — from designing a study with adequate power through analyzing results and avoiding common pitfalls. Your background in field experimental design transfers directly here.

All notebooks use simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `power_analysis.ipynb` | Sample size calculation and power analysis for common test types using `pwr` |
| `ab_test_proportions.ipynb` | Two-sample proportion test for binary outcomes (conversion rates, treatment response) |
| `ab_test_means.ipynb` | Two-sample t-test for continuous outcomes; connecting to basic inference |
| `multiple_testing_correction.ipynb` | Bonferroni, Benjamini-Hochberg (FDR), and when each is appropriate |
| `experiment_design_principles.ipynb` | Randomization, blocking, stratification, and controlling for confounders |
| `sequential_testing.ipynb` | Early stopping and sequential testing; controlling type I error over time |
| `minimum_detectable_effect.ipynb` | Defining and justifying the minimum effect size worth detecting |

---

## Applications by Sector

| Sector | Example |
|---|---|
| **Ecology** | Field experiment design for habitat manipulation; treatment/control plot randomization; testing restoration intervention effects |
| **Healthcare** | Clinical trial design; comparing treatment arms; evaluating screening protocol efficacy |
| **Finance** | Testing impact of a product change on transaction volume; evaluating a new pricing model |
| **Insurance** | Testing a new underwriting rule on claim rates; evaluating a customer communication intervention |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "pwr", "statsmodels"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
