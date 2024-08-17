Gradient Descent is an iterative optimization algorithm that tries to find the optimum value (Maximum/Minimum) of a function. We use it in Linear Regression to **update the parameters of the model to minimize the cost function**.
## How Gradient Descent Works
### Compute Gradient
First we compute the [[Gradient]] of the cost function:
$$\frac{\partial}{\partial w}J(w,b)=\frac{1}{m}\sum_{i=1}^{m}(f_{w,b}(x^{(i)})-y^{(i)})x^{(i)}$$
$$\frac{\partial}{\partial b}J(w,b)=\frac{1}{m}\sum_{i=1}^{m}(f_{w,b}(x^{(i)})-y^{(i)})$$
### Update the Parameters
Then we update the parameters with the Update Sentence:
$$w=w-\alpha \frac{\partial}{\partial w}J(w,b)$$
$$b = b-\alpha \frac{\partial}{\partial b}J(w,b)$$