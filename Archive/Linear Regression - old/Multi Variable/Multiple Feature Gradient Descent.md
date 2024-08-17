[[Multiple Features]]
[[Squared Error Cost Function]]
[[Vectorizatoin]]

---

# Vector Notations
- Parameters
	- $\vec w = [w_1, w_2, ...., w_n]$
	- $b$
- Model
	$f_{\vec w, b}(x)=\vec w.\vec x +b$
- Cost Function
  $J(\vec w, b)$

# Gradient Descent
- $w_j=w_j-\alpha \frac{\partial}{\partial w_j}J(\vec w, b)$
- $b=b-\alpha \frac{\partial}{\partial b}J(\vec w, b)$
Then we Update each feature simultaneously:
- $j=1$ 
  $$w_1=w_1-\alpha \frac{1}{m} \sum_{i=1}^m(\vec x^{(i)}-y^{(i)})x_1^{(i)}$$
- $j=2$
 $$w_2=w_2-\alpha \frac{1}{m} \sum_{i=1}^m(\vec x^{(i)}-y^{(i)})x_2^{(i)}$$
 And so until $j=n$

# Notes
- **Normal Equation :** an Alternative for Gradient Descent.
	- Only for Linear Regression
	- Solve $w,b$ without iterations
	- Slow when number of features is large $> 10,000$
	- It may be used in the back-end of machine learning libraries.
	- Gradient Descent is better