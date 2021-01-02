*K*-means Clustering
================

\*Step 1: Choose the number *K* of clusters.

\*Step 2: Select at random *K* points, the centroid (not necessarily from the dataset).

\*Step 3: Assign each data point to the closet centroid. Form the *K* clusters.

\*Step 4: Compute and place the new centroid of each cluster.

\*Step 5: Reassign each data point to the new closest centroid. If any reassignment took place, then go to Step 4, otherwise this is the final assignment of data points.

# Python Code

## Importing libraries

``` python
import numpy as np
x = np.array([1,2,3])
x[1]
```

    ## 2
