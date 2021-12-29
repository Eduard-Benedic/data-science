# 2.2 Variable Types and Terminology

X - Input Variable
X vector - components can be accessed by subpscripts X<sub>j</sub>
Y - quantitative outputs
G - qualitative outputs (G for group)

Uppercase letters - $X, Y, G$ - reffer to generic aspect of a variable

$x$<sub>$i$</sub> - observed values are written in lowercase

**X** - matrix is in bold

All vectors assumed to be column vectors

$\hat{Y}$ - prediction of output Y

# 2.3.1 Linear models and Least Squares

$$ \hat{Y} = \hat{\beta}_0 + \sum_{j=1}^p X_j\hat{\beta_j} $$

Alternatively we can move the $\hat{\beta}_0$ in the vectors of coefficients and add a 1 to the vector $X$.

$$\hat{Y} = X^T\hat{\beta}$$

Least Squares

Pick coefficients $\beta$ to minimize the **Residual Sum of Squares**.

$$ RSS(\beta) = \sum_{i=1}^N (y_i - x_i^T \beta)^2 $$
$ RSS(\beta) $ - quadratic function of the parameters and its minimum always exists.

$$ RSS(\beta) = (y - \mathbf{X} \beta)^T(y - \mathbf{X}\beta) $$

# 2.3.2 Neaerest-Neighbor Methods

