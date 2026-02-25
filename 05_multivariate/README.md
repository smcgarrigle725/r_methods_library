# Multivariate & Community Analysis

Notebooks covering multivariate methods in R, with a focus on dissimilarity-based approaches from community ecology. These methods are applicable wherever the unit of analysis is a *profile* or *composition* rather than a single variable — species assemblages, patient symptom profiles, customer feature vectors, or portfolio compositions.

All notebooks use built-in or simulated datasets — no downloads required.

> **Note on Python equivalents:** Most dissimilarity-based methods (PERMANOVA, nMDS, ANOSIM) are implemented in R's `vegan` package without close Python equivalents. `scikit-bio` provides partial coverage. Where Python alternatives exist, they are noted within each notebook.

---

## Contents

| Notebook | Description |
|---|---|
| `multivariate_assumptions.ipynb` | Dispersion homogeneity (betadisper), checking multivariate normality; these are the assumption checks that belong before PERMANOVA and dbRDA |
| `pca.ipynb` | Principal components analysis: ordination, biplots, variance explained, and interpretation |
| `nmds.ipynb` | Non-metric multidimensional scaling: stress, ordination plots, and species vectors |
| `permanova.ipynb` | PERMANOVA and pairwise PERMANOVA for testing multivariate group differences |
| `anosim_mantel.ipynb` | ANOSIM for group separation; Mantel test for matrix correlation |
| `dbrda.ipynb` | Distance-based redundancy analysis: constrained ordination with environmental predictors |
| `beta_diversity.ipynb` | Decomposing beta diversity into nestedness vs. turnover components (betapart); important for interpreting PERMANOVA results |
| `indicator_species.ipynb` | IndVal and multipatt for identifying which species characterize each group; pairs naturally with NMDS/PERMANOVA |
| `clustering.ipynb` | Hierarchical clustering and k-means applied to community/compositional data |
| `biplots_visualization.ipynb` | Publication-quality ordination plots with species/variable vectors using `ggplot2` |

---

## Dependencies

```r
install.packages(c("vegan", "ade4", "FactoMineR", "factoextra",
                   "tidyverse", "ggplot2", "cluster"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
