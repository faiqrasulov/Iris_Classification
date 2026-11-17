# Clustering the Iris dataset

> Course assignment from 2023, kept as it was written. The notes under "Reading the result" were added in November 2026.

Clusters the 150 Iris flowers with K-means and Ward hierarchical clustering, and chooses the
number of clusters with the elbow method and silhouette scores.

## Result

| Clusters | Average silhouette |
|---|---|
| 2 | 0.464 |
| 3 | 0.443 |
| 4 | 0.417 |
| 5 | 0.415 |
| 6 | 0.396 |

## Reading the result

- **The notebook picks 5 clusters, and that is not what its own numbers say.** The silhouette is
  highest at 2 and 3, and the data has 3 species. Five came from reading the elbow plot too
  generously.
- The species labels are in the file but are not used to check the clusters. An adjusted Rand
  index against species is the missing check.

## Files

| File | Content |
|---|---|
| `Iris_Classification.ipynb` | Analysis |
| `Iris_Classification.html` | Rendered copy |
| `Iris.csv` | The dataset |
| `About.txt` | Original brief |
