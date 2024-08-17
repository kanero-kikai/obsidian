Mean Squared Error (MSE) is the [[Cost Function]] used in Linear Regression. As the name says, we calculate the **Average** of the **Squared Error** between our **prediction** $\hat y~/~f_{w,b}(x)$ and the original **target** $y$.
## Equation
$$J(w,b)=\frac{1}{2m}\sum_{i=1}^{m}{(f_{w,b}(x^{(i)})-y^{(i)})^2}$$
- $J(w,b)$ : the MSE cost function for the parameters $w, b$.
  Note that the cost function is for the whole dataset used. As we use **summation** over the entire data from $i=1$ to $m$.
- $\frac{1}{2m}\sum_{i=1}^{m}{(...)^2}$ : the average (mean) of the the squared error. (we use 2 for neater results, as it will get cancelled in the derivation process in the gradient descent process).
- $f_{w,b}{(x^{(i)})}-y^{(i)}$ : the error for a single training set.