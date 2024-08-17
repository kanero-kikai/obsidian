[[Squared Error Cost Function]]

---
We use Gradient Descent to minimize any function, $min_{w_1, w_n, b}~J(w_1, w_n, b)$ as $w_1:w_n, b$ are the parameters.
### How the Gradient Descent algorithm works?
- Choose a starting point (The initial value we set to $w,b$) 
- Look around $360\degree$ 
- Choose which direction is faster to reach the minimum 
- Move a little step
- Repeat the process
![[Untitled 1.png|693]]
- There might be many minimum values (local minimums), and if the algorithm finds one it will stick with it. Until we restart it with another initial values.
  And this because the slope at a local minimum is 0. So the derivative of the cost function will be $\frac{\partial}{\partial b} J(w,b)=0$. And if you substituted with this in the [[#Update Statement]] you will end up with $w = w$. Means nothing is changing. 
# Gradient Descent algorithm
> [!info] The = operator can mean 2 things
> - Assignment: Like in code, the value on the right is assigned to the variable on the left
> - Truth Assertion: Like in normal math

## Update Statement
$$
w=w-\alpha\frac{\partial}{\partial w} J(w,b)
$$

- $w$ *on the left*: is the new step the algorithm will take.
- $w$ *on the right*: is the old step.
- $\alpha :$ The learning rate.
	- $\in [0,1]$
	- If the value is small, the algorithm will take small steps 
	- If the value is large, the algorithm will take giant steps (aggressive gradient descent)
- $\frac{\partial}{\partial w} J(w,b) :$ The derivative of the cost function, and it's the direction the algorithm will take.
And same goes for $b$
$$ 
b=b-\alpha\frac{\partial}{\partial b} J(w,b)
$$
<u>These two process will repeat until convergence (Until their value aren't changing in a significant way).</u>
### Simultaneous Update
We need to simultaneously update the two values, means we need to update them at the same time. 
$$
temp\_w=w-\alpha\frac{\partial}{\partial w} J(w,b) 
$$
$$
temp\_b=b-\alpha\frac{\partial}{\partial b} J(w,b)
$$
$$
w=temp\_w
$$
$$
b=temp\_b
$$
> [!warning] Incorrect way to update the values.
> $$temp\_w=w-\alpha\frac{\partial}{\partial w} J(w,b) $$
> $$w=temp\_w$$
> $$temp\_b=b-\alpha\frac{\partial}{\partial b} J(w,b)$$
> $$b=temp\_b$$
> Because the value of $w$ will affect the value of $b$.

# Gradient Descent intuition
## Cost function derivative

![[Untitled 2.png|635]]
## Learning rate
- If the learning rate is **Too small**, The algorithm **will Work**, but **very Slow**, as it's taking very small steps.
![[Gradient Descent-20240610105745969.png|218]]
- If the learning rate is **Too Large**, It will take huge steps that will **get bigger and bigger by time**. And the cost function will increase. And the model will **not converge**, it may even diverge.    
![[Gradient Descent-20240610105805281.png|210]]
# Notes
- **The steps isn't the same size :** Because when we get closer to the minimum, the slope decreases, which means the the cost function derivative $\frac{\partial}{\partial b} J(w,b)$ is decreasing. And $w$ will change is smaller values. 
  ![[Gradient Descent-20240610111020208.png|216]]
  
- The cost function we using is **squared error function**, and it’s a **convex** function (bowl shaped, have only **one global minimum** and no local minimums). So don’t worry about the local minimums.
- The gradient descent we are using is called **Batch Gradient** Descent as we are using the entire dataset each time we take a step Look at the derivatives, we are summing up from $i=1 ~to~m$, which is all the dataset.