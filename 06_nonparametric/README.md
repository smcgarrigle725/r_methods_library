# Nonparametric Methods

Notebooks covering nonparametric hypothesis tests in R — methods that make no assumptions about the underlying distribution of the data. These are appropriate when normality assumptions are violated, sample sizes are small, or data are ordinal.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `rank_tests_two_groups.ipynb` | Mann-Whitney U test and Wilcoxon signed-rank test as nonparametric alternatives to t-tests |
| `rank_tests_multiple_groups.ipynb` | Kruskal-Wallis test and Dunn's post-hoc test as nonparametric alternatives to one-way ANOVA |
| `correlation_nonparametric.ipynb` | Spearman rank correlation and Kendall's tau |
| `permutation_tests.ipynb` | Permutation-based inference: concept, implementation, and when to use it |
| `normality_tests.ipynb` | Shapiro-Wilk, Kolmogorov-Smirnov, and Anderson-Darling tests; Q-Q plots |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "coin", "nortest",
                   "dunn.test", "rstatix", "ggpubr"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
