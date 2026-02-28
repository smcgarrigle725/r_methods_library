# 12 · Clustering

Unsupervised methods for discovering structure in unlabelled data. Covers the full workflow: choosing a method, selecting k, validating results, and — critically — profiling clusters to determine whether they are scientifically meaningful.

| Notebook | Description |
|---|---|
| `kmeans_R.ipynb` | k-means; elbow, silhouette, and gap statistic for choosing k; pitfalls of spherical cluster assumption |
| `hierarchical_clustering_R.ipynb` | Agglomerative clustering; linkage methods; dendrograms; Gower distance for mixed-type data |
| `dbscan_R.ipynb` | Density-based clustering; k-NN distance plot for eps selection; HDBSCAN for variable-density clusters |
| `gaussian_mixture_models_R.ipynb` | Soft assignments; covariance model selection via BIC; uncertainty of assignment; `mclust` |
| `cluster_validation_R.ipynb` | Silhouette, Calinski-Harabasz, Davies-Bouldin, Dunn; external validation with ARI |
| `dimensionality_reduction_R.ipynb` | PCA → t-SNE/UMAP workflow for visualising high-dimensional data before and after clustering |
| `cluster_profiling_R.ipynb` | Interpreting clusters: heatmaps, Kruskal-Wallis, effect sizes, naming, boundary observations |

**Key packages:** `cluster`, `factoextra`, `dbscan`, `mclust`, `fpc`, `uwot`, `Rtsne`

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "cluster", "factoextra",
                   "dbscan", "mclust"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
