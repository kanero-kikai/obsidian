# Linear Regression Model
## Notations
- $x :$ "Input" variable / feature
- $y :$ "Output" variable / target
- $m :$ number of training examples
- $w,~b :$ The Parameters
- $\alpha :$ The learning rate


## [[Univariate Linear Regression Model.|The Model]]
$$
f_{w,b}(x)=wx+b
$$
## [[Squared Error Cost Function]]
$$J(w,b)=\frac{1}{2m}\sum_{i=1}^m(f_{w,b}(x^{(i)})-y^{(i)})^2$$
## [[Git/Archive/Linear Regression - old/Univariate/Gradient Descent]]
### Algorithm
$$w=w-\alpha \frac{\partial}{\partial w}J(w,b)$$
$$b=b-\alpha\frac{\partial}{\partial b}J(w,b)$$
### Derivatives
$$\frac{\partial}{\partial w}J(w,b)=\frac{1}{m}\sum_{i=1}^m(f_{w,b}(x^{(i)})-y^{(i)})x^{(i)}$$
$$\frac{\partial}{\partial b}J(w,b)=\frac{1}{m}\sum_{i=1}^m(f_{w,b}(x^{(i)})-y^{(i)})$$