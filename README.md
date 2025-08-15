# Mall Customers Clustering with K-Means

This project applies **K-Means Clustering** on the `Mall_Customers.csv` dataset to segment customers based on their **Annual Income** and **Spending Score**.  
The goal is to group customers into distinct clusters for targeted marketing strategies.

## Steps Performed

1. **Load and Preprocess Data**
   - Loaded `Mall_Customers.csv` dataset.
   - Selected relevant features: `Annual Income (k$)` and `Spending Score (1-100)`.
   - Standardized the features using `StandardScaler`.

2. **Dimensionality Reduction (Optional)**
   - Applied **PCA** for visualization in 2D space (useful if more than 2 features are used).

3. **Finding Optimal Number of Clusters**
   - Used the **Elbow Method** to plot **Inertia** vs. **Number of Clusters (K)**.
   - Determined the best K for clustering.

4. **Fit K-Means Model**
   - Trained K-Means using the optimal K value.
   - Assigned cluster labels to each customer.

5. **Visualize Clusters**
   - Plotted the clusters with distinct colors.
   - Marked cluster centroids.

6. **Evaluate Clustering**
   - Used **Silhouette Score** to measure the quality of clustering.

## Requirements

Install dependencies with:
```bash
pip install pandas numpy matplotlib scikit-learn
