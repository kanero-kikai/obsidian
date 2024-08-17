[[Multiple Features]]

---

Let's say we have:
- $\vec w = [w_1, w_2, w_3]$ 
- $b$
- $\vec x = [x_1, x_2, x_3]$
- $n = 3$
And our model will be:
$$f_{\vec w, b}(x)=w_1x_1+w_2x_2+w_3x_3+b$$
And this is how to write it in `NumPy`
```python
w = np.array([w1, w2, w3])
b = b
x = np.array([x1, x2, x3])
```

**How can we implement our model?**
## Without Vectorizatoin
### By hand
We can write it like:
```python
f = w[0]*x[0] + w[1]*x[1] + w[2]*x[2] + b
```
It it won't be efficient if we got like 100 features.
### Summation & For loop
We can rewrite the model as:
$$f_{\vec w, b}(x)=\sum_{j=1}^{n}(w_jx_j)+b$$
And in code
```python
f = 0
for j in range(n):
	f += w[j]*x[j]
f += b
```
But this is also inefficient Because it's slow
## With Vectorization
The model is:
$$ f_{\vec w,b}(x)=\vec w.\vec x+b $$
And the code is:
```python
f = np.dot(w, x) + b
```
Very simple! But also much faster because `NumPy` can use **Parallel Hardware**, Instead of doing it step by step like the previous methods.

*Note: `.dot()` method is for dot product*
### Why Vectorization is fast
Here is a comparison
![[Vectorizatoin-20240610181846011.png]]
As you can see, Without vectorization, the computer do it step by step. But with vectorization the computer multiply all value at the same time.

Another example when we Use update statement in gradient descent algorithm
![[Vectorizatoin-20240610182339086.png]]
With Vectorization all the features are updated in the same time in one step.