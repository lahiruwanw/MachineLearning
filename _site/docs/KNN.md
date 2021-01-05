*K*-Nearest Neighbors (K-NN)
================

*K*-Nearest Neighbors (K-NN) is a non-linear classification method. Given a positive integer *K*, the K-NN classifier identifies the *K* observations (represented the set as *N*<sub>0</sub>) nearest to an observation *x*<sub>0</sub>. It then estimates the conditional probability for category *j* as

![equation](https://latex.codecogs.com/gif.latex?%5Ctext%7BPr%7D%20%28Y%3Dj%7CX%3Dx_0%29%20%3D%20%5Cfrac%7B1%7D%7BK%7D%20%5Csum_%7Bi%20%5Cin%20N_0%7D%20I%28y_i%20%3D%20j%29.)

The observation *x*<sub>0</sub> assign to the category *j* with the largest conditional probability. Here are the steps of the K-NN classifier.

-   Step 1: Choose the number *K* of neighbors.

-   Step 2: Take the *K* nearest neighbors of the new observation *x*<sub>0</sub> using the distance measure (euclidean distance etc.)

-   Step 3: Among these *K* neighbors, count the number of observations in each category.

-   Step 4: Assign the new observation to the category with the largest probability.

[Python Code](k_nearest_neighbors.ipynb)

[R Code](knn.R)

The choice of *K* has a drastic effect on the *K*-NN classifier. When *K* = 1, the decision boundary is overly flexible, but as *K* grows, the decision boundary is less flexible, and that is close to linear. When *K* is large, the *K*-NN classifier has low variance but high bias.
