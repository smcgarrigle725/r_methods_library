# 13 · Dimensionality Reduction

Methods for compressing high-dimensional data into fewer dimensions while preserving structure. The folder progresses from interpretable linear methods (PCA, FA) through non-linear visualisation tools (t-SNE, UMAP) to ecologically specialised ordination (CA, nMDS) and high-dimensional sparse approaches.

| Notebook | Description |
|---|---|
| `pca_R.ipynb` | Loadings, scree plots, biplots, contribution plots, and out-of-sample projection |
| `factor_analysis_R.ipynb` | EFA vs. PCA; latent constructs; parallel analysis for factor number; oblique rotation |
| `tsne_R.ipynb` | t-SNE; perplexity sensitivity; colouring by feature; why inter-cluster distances are meaningless |
| `umap_R.ipynb` | UMAP; parameter sensitivity grid; out-of-sample embedding with `umap_transform`; batch confounding |
| `correspondence_analysis_R.ipynb` | CA for contingency tables and species × site matrices; MCA for multiple categorical variables |
| `nmds_R.ipynb` | nMDS with Bray-Curtis dissimilarity; stress and Shepard diagram; `envfit` vectors; PERMANOVA; metric MDS (PCoA) |
| `sparse_methods_R.ipynb` | Sparse PCA for interpretable loadings when p >> n; ICA for non-Gaussian source separation |

**Key packages:** `prcomp`, `psych`, `Rtsne`, `uwot`, `FactoMineR`, `vegan`, `sparsepca`, `fastICA`

> **Note:** `dimensionality_reduction_R.ipynb` in `12_clustering` covers PCA + t-SNE + UMAP as an integrated visualisation workflow for clustering. The notebooks here go deeper on each method individually.

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "FactoMineR", "factoextra",
                   "Rtsne", "umap", "psych"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
