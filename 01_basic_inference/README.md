# 01 · Basic Inference

Foundational hypothesis testing and estimation. These notebooks establish the vocabulary and workflow used throughout the library — effect sizes, confidence intervals, and the distinction between statistical and practical significance.

| Notebook | Description |
|---|---|
| `t_tests_R.ipynb` | One-sample, two-sample, and paired t-tests; Welch vs. Student; Cohen's d |
| `anova_R.ipynb` | One-way and two-way ANOVA; post-hoc tests (Tukey, Bonferroni); effect sizes |
| `chi_square_R.ipynb` | Chi-squared goodness-of-fit and test of independence; Fisher's exact test |
| `confidence_intervals_R.ipynb` | CI construction, interpretation, and bootstrap CIs for any statistic |

**Key packages:** `stats`, `effectsize`, `boot`, `rstatix`

## Dependencies

```r
install.packages(c("tidyverse", "ggpubr", "car", "effectsize", "rstatix", "pwr"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
