# Clustering

Notebooks covering unsupervised clustering methods in R — algorithms that group observations by similarity without predefined labels. Clustering is used to discover natural groupings in data: species assemblages, patient subtypes, customer segments, or risk cohorts.

All notebooks use built-in or simulated datasets — no downloads required.

---

## Contents

| Notebook | Description |
|---|---|
| `kmeans.ipynb` | k-means clustering; choosing k with the elbow method and silhouette scores |
| `hierarchical_clustering.ipynb` | Agglomerative hierarchical clustering; dendrograms and linkage methods |
| `dbscan.ipynb` | DBSCAN for density-based clustering; handling noise and irregular cluster shapes |
| `gaussian_mixture_models.ipynb` | Gaussian mixture models with `mclust`; probabilistic cluster assignment |
| `cluster_validation.ipynb` | Internal validation metrics: silhouette width, Calinski-Harabasz, Davies-Bouldin |
| `dimensionality_reduction.ipynb` | PCA, UMAP, and t-SNE for visualising high-dimensional data before and after clustering; these are almost always used together with clustering in practice and the workflow of "reduce → cluster → visualise" deserves its own notebook. Distinct enough from the clustering methods themselves |
| `cluster_profiling.ipynb` | Interpreting and describing clusters after assignment: heatmaps of feature means, statistical tests between clusters, naming/labelling strategies; the step most notebooks skip entirely but that determines whether clustering results are actually usable |

---

## Dependencies

```r
install.packages(c("tidyverse", "ggplot2", "cluster", "factoextra",
                   "dbscan", "mclust"))
```

Notebooks run in Jupyter via the R kernel. See the [repo root README](../README.md) for IRkernel setup instructions.

---

*Part of [r_methods_library](https://github.com/samantha-mcgarrigle/r_methods_library)*
