## Clustering with K-Means

### Tools & Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib
- kneed (for optimal K detection)


### Steps Performed

#### 1. **Data Loading & Exploration**
- Loaded dataset using `pandas`.
- Checked for null values and basic statistics.
- Selected relevant features for clustering.

#### 2. **Data Visualization**
- Plotted scatter plot of `Annual Income` vs `Spending Score` to visualize customer distribution.

#### 3. **Elbow Method to Find Optimal K**
- Used `KMeans` with cluster sizes from 1 to 10.
- Plotted inertia (WCSS) to observe the "elbow".
- Used `KneeLocator` to detect the optimal number of clusters.
- **Optimal K found: 5**

#### 4. **K-Means Clustering**
- Fitted KMeans model with `n_clusters=5`.
- Assigned cluster labels to each customer.
- Appended cluster labels to the original dataset.

#### 5. **Cluster Visualization**
- Used `seaborn` to color-code clusters.
- Plotted K-Means cluster centroids on the scatter plot.

#### 6. **Evaluation using Silhouette Score**
- Calculated Silhouette Score to evaluate clustering quality.
- **Silhouette Score: 0.55** (indicates moderately good clustering)
  
---
