# Basic Statistical Inference

Notebooks covering foundational hypothesis testing methods in R. These form the basis of more complex analyses and are directly applicable across ecological, clinical, financial, and insurance contexts.

All notebooks use built-in R datasets — no downloads required. Each follows a consistent structure: assumptions checklist, inline assumptions testing, analysis, interpretation, and common pitfalls.

---

## Contents

| Notebook | Description |
|---|---|
| `t_tests.ipynb` | One-sample, independent two-sample (Welch's & Student's), and paired t-tests with effect sizes |
| `anova.ipynb` | One-way and two-way ANOVA, post-hoc tests (Tukey HSD, Bonferroni), and assumption checking |
| `chi_square_fisher.ipynb` | Chi-square test of independence, goodness-of-fit test, and Fisher's exact test for small samples |
| `confidence_intervals_effect_sizes.ipynb` | Confidence interval construction, Cohen's d, eta-squared, and power analysis |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggpubr", "car", "effectsize", "rstatix", "pwr"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
