# Lab-5-Clustering-Techniques-Using-DBSCAN-and-Hierarchical-Clustering
Lab 5: Clustering Techniques Using DBSCAN and Hierarchical Clustering

# MSCS 634: Lab 5 - Clustering Techniques Using DBSCAN and Hierarchical Clustering

## Purpose
The purpose of this lab was to experiment with clustering techniques using Hierarchical Clustering and DBSCAN on the Wine dataset. the main goal was to understadn how different these approaches are in terms of, parameter sensitivity and clustering results.

## Key Insights
1. **Hierarchical Clustering**:
   - Formed three clusters consistently, as visualized in scatter plots and the dendrogram.
   - Results showed a clear hierarchical relationships.
    

2. **DBSCAN**:
   - It was able to identify noise points and clusters of varying density.
   - Results indicates that it was depend on parameters like `eps` and `min_samples`.
   - Metrics like Silhouette Score returned `NaN` probably because of unclustered noise. 

## Challenges
- The main challenge is that it was difficult to fine-tuning DBSCAN parameters to achieve meaningful clusters.

## Here is the detailed analysis

1. **Hierarchical Clustering**:
   - The codes above for hierarchical clustering generated evenly distributed clusters and visualized them in scatter plots and the dendrogram.
   - We have learned that Hierarchical clustering model is effective for datasets with clear hierarchical relationships.

2. **DBSCAN**:
   - DBSCAN was able to identify noise datapoints and clusters with irregular shapes.
   - However, it was highly sensitive to `eps` and `min_samples`. We also noted taht there is possibly issues of suboptimal parameters which led to clusters being undefined and metrics like Silhouette Score returning `NaN`.

3. **Comparative Insights**:
   - Comparing the two models revels that Hierarchical clustering is reliable for structured data and it is very easy to interpret with dendrograms.
   - On the other hand, DBSCAN is most suitable for datasets with noise or varying densities despite the issue with parameters choice.

4. **Conclusion**:
   - We therefore conclude that Hierarchical clustering is better choice when dealing with structured and evenly distributed datasets and DBSCAN is more effective when handling noise and irregular clusters. 
