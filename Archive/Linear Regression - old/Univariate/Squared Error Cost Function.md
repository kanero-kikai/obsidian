[[Univariate Linear Regression Model.]]

---
We use it to calculate the error of our prediction, or how far our prediction from the actual value.

For Linear Regression problems and most Regression problems we use:
## Squared Cost Function
$$
J(w,b)=\frac{1}{2m}\sum_{i=1}^m(\hat y^{(i)}-y^{(i)})^2
$$
or: 
$$
J(w,b)=\frac{1}{2m}\sum_{i=1}^m(f_{w,b}(x^{(i)})-y^{(i)})^2
$$
- $J :$ is the cost function.
- $w,~b :$ are the parameters
- $\frac{1}{2m} :$ is the average, but we use 2 for neater results, as this 2 will get cancelled in the derivation process in the gradient descent. 
- The rest of the function is the sum of squared errors.
### Goal
We want to **minimise** the cost function. We want to make $w,~b$ makes the cost function as small as possible.
We want $minimise_{w,b}J(w,b)$.
#### Notes
- The model (the function) depends on the input. As $f(x)$ is a function of $x$ (input).
- The cost function depends on the parameters. As $J(w,b)$ is a function of $w,b$ (parameters).

