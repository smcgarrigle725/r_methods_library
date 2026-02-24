# Dimensionality Reduction

Notebooks covering methods for reducing high-dimensional data to fewer dimensions while preserving meaningful structure. Used for visualization, noise reduction, feature extraction, and as preprocessing for downstream modeling.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `pca.ipynb` | Principal components analysis: variance explained, loadings, biplots, and scree plots |
| `factor_analysis.ipynb` | Exploratory factor analysis; comparing to PCA and when to prefer it |
| `tsne.ipynb` | t-SNE for nonlinear dimensionality reduction and cluster visualization |
| `umap.ipynb` | UMAP as a faster, more scalable alternative to t-SNE |
| `correspondence_analysis.ipynb` | Correspondence analysis for categorical/count data (e.g. species × site matrices) |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "FactoMineR", "factoextra",
                   "Rtsne", "umap", "psych"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
