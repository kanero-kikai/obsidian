Here we will discuss the dataset and the model (function).
==1 Feature -> Univariate==
# Some Notations
- $x :$ "Input" variable / feature
- $y :$ "Output" variable / target
- $m :$ number of training examples
- $(y,~x) :$ Single training example
- $(y^{(i)},~x^{(i)}) :$ $i^{th}$ training example. *(We put $i$ in ())

![[Untitled.png]]

- $f :$ The function the training algorithm creates. Also called **Hypothesis**, and it's our model!
  This function takes the input $x$ and predict estimated $y$ value denoted as $\hat y$. 

# Linear Regression Function
$$
f_{w,b}(x)=wx+b
$$
- $w,~b :$ are constants not variables like $x$.
	- $w :$ slope
	- $b :$$~y-$intercept
- $w,~b :$ are the parameters of the model. They are the variables that the training algorithm tries to adjust during the training to improve the model. 
  Also called (coefficients, weights).
  