# 05 · Multivariate Analysis

Methods for analysing multiple response variables simultaneously — essential for community ecology, morphometrics, and any setting where outcomes are inherently multidimensional.

| Notebook | Description |
|---|---|
| `manova_R.ipynb` | MANOVA; Pillai, Wilks, Hotelling-Lawley, Roy statistics; follow-up univariate tests; canonical discriminant scores |
| `discriminant_analysis_R.ipynb` | LDA and QDA for group separation and classification; structure matrix; LOO-CV accuracy |
| `cluster_analysis_intro_R.ipynb` | Overview of clustering approaches; distance metrics; data preparation |
| `pca_intro_R.ipynb` | PCA for multivariate data reduction; scores and loadings |
| `canonical_correlation_R.ipynb` | CCorA relating two continuous variable sets; canonical loadings; redundancy index |
| `rda_R.ipynb` | Redundancy analysis (linear constrained ordination); Hellinger-transformed species data; variance partitioning; forward selection |
| `multivariate_regression_R.ipynb` | Multiple responses; MANOVA as regression; coefficient matrices |
| `hotelling_t2_R.ipynb` | Hotelling's T² for multivariate group comparisons |
| `profile_analysis_R.ipynb` | Repeated measures multivariate; parallelism, levels, flatness tests |
| `procrustes_R.ipynb` | Procrustes analysis; shape comparison; matrix superimposition |
| `multivariate_normality_R.ipynb` | Testing MVN; Mardia, Royston, Henze-Zirkler tests; QQ plots |

**Key packages:** `MASS`, `candisc`, `CCA`, `MVN`, `vegan`, `mvnormtest`, `car`

---

## Dependencies

```r
install.packages(c("vegan", "ade4", "FactoMineR", "factoextra",
                   "tidyverse", "ggplot2", "cluster"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
