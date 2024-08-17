# Notations
![[Multiple Features-20240610145125967.png]]
- $x_j=j^{th}$ feature
- $n :$ number of features
- $\vec x^{(i)} :$ vector (list) of features of $i^{th}$ training example
- $x_j^{(i)} :$ value of feature $j$ in $i^{th}$ training example
# Multiple Linear Regression Model
$$f_{w,b}(x)=w_1x_1+w_2x_2+...+w_nx_n+b$$
### Parameters
- $w :$ Weights, so the weight of feature $x_1$ is $w_1$
- $b :$ Bias, so if all weights or features are $0$, we still have bias $b$
### Another Shape
We can represent all $w$ as:
$$ \vec w=[w_1~~w_2~~...~~w_n] $$
And $x$ as:
$$ \vec x=[x_1~~x_2~~...~~x_n] $$
And rewrite the model as:
$$ f_{\vec w,b}(x)=\vec w.\vec x+b $$
