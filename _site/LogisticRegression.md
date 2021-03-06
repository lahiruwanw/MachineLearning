Classification
================

In classification, we predict the qualitative response or the category,
which means we classify the observations to a category or a class. Most
of the classification methods first predict the probability that the
observation belongs to each of the categories and then assign the label
of the category which has the highest probability. There are two main
types of classification methods:

1.  Linear Classification

<!-- end list -->

  - Logistic Regression
  - Support Vector Machine (SVM)

<!-- end list -->

2.  Non-linear Classification

<!-- end list -->

  - \(K\)-nearest neighbor (K-NN)
  - Kernel Support Vector Machine (SVM)
  - Random Forests.

# Logistic Regression

In logistic regression insted of modeling the response \(Y\) directly,
we model the probaility that \(Y\) belongs to a particular category. For
convenience we are using the generic 0/1 coding for the response. Using
a linear regression model we model the probability
\[ p = \text{Pr}(Y=1|X) = \beta_0 + \beta_1 X.\] We must model \(p\)
using a function that gives output between 0 and 1 for all the values of
X. In logistic regression, we use the logistic function

![equation](https://latex.codecogs.com/gif.latex?p%20%3D%20%5Cfrac%7Be%5E%7B%5Cbeta_0%20+%20%5Cbeta_1%20X%7D%7D%7B1%20+%20e%5E%7B%5Cbeta_0%20+%20%5Cbeta_1%20X%7D%7D.)

Then

![equation](https://latex.codecogs.com/gif.latex?%5Cfrac%7Bp%7D%7B1-p%7D%20%3D%20e%5E%7B%5Cbeta_0%20+%20%5Cbeta_1%20X%7D%2C)

where the quantity \(p/(1-p)\) is called the odds, and can take on any
value between 0 and \(\infty\). By taking the logarithm of both sides

![equation](https://latex.codecogs.com/gif.latex?%5Ctext%7Bln%7D%20%5Cleft%28%5Cdfrac%7Bp%7D%7B1-p%7D%5Cright%29%20%3D%20%5Cbeta_0%20+%20%5Cbeta_1%20X.)

The left-hand side is called the log-odds or logit and this logit is
linear in \(X\).

[Python Code](logistic_regression.ipynb)

[R Code](logistic_regression.R)
