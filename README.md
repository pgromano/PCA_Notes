# Principal Component Analysis

A demo of 3 PCA examples is given in [PCA Demo Notebook](PCA\ Demo.ipynb).

> "By eye, it is clear that there is a nearly linear relationship between the x and y variables. This is reminiscent of the linear regression data we explored in In Depth: Linear Regression, but the problem setting here is slightly different: rather than attempting to predict the y values from the x values, the unsupervised learning problem attempts to learn about the relationship between the x and y values.

> In principal component analysis, this relationship is quantified by finding a list of the principal axes in the data, and using those axes to describe the dataset."

> – Jake VanderPlas

PCA is a spectral decomposition method which solves for the eigenvectors (principal components) of the covariance matrix:

$${\displaystyle \Sigma _{ij}=\mathrm {cov} (X_{i},X_{j})=\mathrm {E} {\begin{bmatrix}(X_{i}-\mu _{i})(X_{j}-\mu _{j})\end{bmatrix}}=\mathrm {E} {\begin{bmatrix}X_{i}X_{j}\end{bmatrix}}-\mu _{i}\mu _{j}}$$

The matrix $\mathbf{R}$, where each column is an eigenvector of the covariance matrix, with associated eigenvalues $\lambda$ satisfies the condition

$$\mathbf{\Sigma} \propto \mathbf{X}^T \mathbf{X} = \mathbf{R} \mathbf{\Lambda} \mathbf{R}^T$$

where $\mathbf{\Lambda}$ is the diagonal matrix form of the eigenvalues.

PCA is a linear transformation which we can use to change the data $\mathbf{X}$ into an orthogonal coordinate system $\mathbf{T}$. 

$$\mathbf{T} = \mathbf{X} \mathbf{R}$$

The variance of this projected data is maximized by the first axis (principal component), and so on in descending order.

* PCA is a way to spread data out on "natural" axes. 
* Clusters in PCA space can be easier to work with, in particular when classifying noisey data.
* Axes may be hard to interpret directly

# References

1. https://en.wikipedia.org/wiki/Principal_component_analysis
1. https://jakevdp.github.io/PythonDataScienceHandbook/05.09-principal-component-analysis.html

# Interactive Demos

1. http://setosa.io/ev/principal-component-analysis/
1. https://stats.stackexchange.com/questions/2691/making-sense-of-principal-component-analysis-eigenvectors-eigenvalues

