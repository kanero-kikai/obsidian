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
- $a$ : The [[Learning Rate]] 
Then we keep updating the parameters until **Convergence**. Until the values aren't changing in a significant way.
## Notes
### Simultaneous Update
We must update the parameters simultaneously. Because the gradient of the cost function for each parameter depends on the two parameters not one.
So we first compute the two gradients, and then update the parameters.
Or we do this:
```python
temp_w = w - a * dj_dw
temp_b = b - a * dj_db
w = temp_w
b = temp_b
```
### How do Parameters Converge?
![[Untitled 2.png]]
This is a graph of the cost of $w$ and the value of $w$. The **Convergence** will be where the cost function is the least, the **minimum**.
If the the value of $w$ is on the right side of the minimum, the slope will be positive and the value of $w$ will decrease moving to the left.
And if the value where on the left side, the slope will be negative and the value of $w$ will be increased moving to the right
### Steps aren't the same size
**The steps isn't the same size :** Because when we get closer to the minimum, the slope decreases, which means the the cost function derivative $\frac{\partial}{\partial b} J(w,b)$ is decreasing. And $w$ will change is smaller values. 
![[Gradient Descent-20240610111020208.png|216]]
