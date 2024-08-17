# Learning Curve

![[Making sure that Gradient Descent is working correctly-20240703102846725.png|522]]
This is the **learning curve**, Relation between **Cost Functions** and **Number of Iterations** of gradient descent.

The  curve should be decreasing until **convergence** (The curve stop decreasing and become a line), but if it after any iteration increased, This means that:
- The learning rate $\alpha$ is chose poorly (probably it's large)
- There is a bug in the code
# Automatic Convergence Test
Let $\epsilon$ be $10^{-3}$ 
If $J(\vec w,b)$ decreases by $\leq \epsilon$ in one iteration, declare **Convergence**.

But the curve is better, because choosing the right $\epsilon$ is hard, and the curve gives some advanced warning if the gradient is not working well.