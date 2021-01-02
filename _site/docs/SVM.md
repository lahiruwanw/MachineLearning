Support Vector Machines
================

The support vector machine (SVM) is a group of classification algorithms that include a veriety of parametric and non-parametric models. The parametric models include straight lines and similar regression lines. The non-parametric models include a variety of kernel smoothing techniques.

## The advantages of support vector machines

-   Effective in high dimensional spaces.

-   Still effective in cases where number of dimensions is greater than the number of samples.

-   Uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.

-   Versatile: different Kernel functions can be specified for the decision function. Common kernels are provided, but it is also possible to specify custom kernels.

## The disadvantages of support vector machines

-   If the number of features is much greater than the number of samples, avoid over-fitting in choosing Kernel functions and regularization term is crucial.

-   SVMs do not directly provide probability estimates, these are calculated using an expensive five-fold cross-validation (see Scores and probabilities).
