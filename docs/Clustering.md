Clustering
================

In clustering, we seek to partition the data into distinct groups so
that the observations within each group are quite similar to each other,
while observations in different groups are quite different from each
other. The two-best known clustering approaches:

1.  \(K\)-means clustering
2.  Hierarchical clustering

In \(K\)-means clustering, we seek to group the observations in to a
pre-specified \(K\) number of clusters. On the other hand, in
hierarchical clustering we produce tree-like visual representation of
the observations, called a dendrogram, that allows us to obtain the
clustering for each possible number of clusters, from 1 to \(n\) (total
number of observations).

# \(K\)-means clustering

To perform \(K\)-means clustering, we must first specify the desired
number of clusters \(K\), then the \(K\)-means algorithm will assign
each observation to exactly one of the \(K\) clusters. The steps of
\(K\)-means algorithm are given.

  - Step 1: Choose the number \(K\) of clusters.

  - Step 2: Select at random \(K\) points, the centroid (not necessarily
    from the dataset).

  - Step 3: Assign each data point to the closet centroid. Form the
    \(K\) clusters.

  - Step 4: Compute and place the new centroid of each cluster.

  - Step 5: Reassign each data point to the new closest centroid. If any
    reassignment took place, then go to Step 4, otherwise this is the
    final assignment of data points.

[Python Code](k_means_clustering.ipynb)

[R Code](k_means_clustering.R)

# Hierachical Clustering

Hierarchical clustering is an alternative approach which does not
require to specify pre-defined number of clusters upfront. There are two
clustering approaches bottom-up or agglomerative clustering and here I
used agglomerative clustering approach. The steps of hierarchical
clustering algorithm are given.

  - Step 1: Make each observation a single-observation cluster. This
    forms \(n\) clusters (\(n\) - total number of observations).

  - Step 2: Take the two closest observations and make them one cluster.
    Now this forms \(n-1\) clusters.

  - Step 3: Take the two closest clusters and make them one cluster. Now
    this forms \(n-2\) clusters.

  - Step 4: Repeat Step 3 until there is only one cluster.

[Python Code](hierarchical_clustering.ipynb)

[R Code](hc.R)

The advantage of \(K\)-means clustering is it is simple to understand,
easily adaptable and works well on small and large datasets. The main
disadvantage is you need to choose the number of clusters \(K\). The
advantage of hierarchical clustering is that the optimal number of
clusters can be obtained by the model itself using the dendrogram. But,
the hierarchical clustering is not appropriate for large datasets.
