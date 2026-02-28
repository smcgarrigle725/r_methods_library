# 06 · Non-Parametric Methods

Rank-based and distribution-free alternatives for when data are ordinal, heavily skewed, or too small for distributional assumptions to hold.

| Notebook | Description |
|---|---|
| `wilcoxon_tests_R.ipynb` | Wilcoxon signed-rank and Mann-Whitney U; rank-biserial correlation |
| `kruskal_wallis_R.ipynb` | Kruskal-Wallis one-way test; Dunn post-hoc with FDR correction |
| `friedman_test_R.ipynb` | Friedman test for repeated measures; Conover post-hoc |
| `spearman_kendall_R.ipynb` | Rank correlations; Spearman's ρ, Kendall's τ, and their CIs |
| `permutation_tests_R.ipynb` | Permutation tests for any test statistic; building custom null distributions |

**Key packages:** `stats`, `coin`, `NSM3`, `rstatix`

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "coin", "nortest",
                   "dunn.test", "rstatix", "ggpubr"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
