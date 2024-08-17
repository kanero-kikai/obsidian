[[Multiple Feature Gradient Descent]]
[[Git/Archive/Linear Regression - old/Univariate/Gradient Descent]]
___

If the feature value range in big (*ex:* 1000 ~ 8000000). The Gradient Descent will take long time bouncing back and forth to get the right parameters.
But if the range was small (*ex:* 0 ~ 1). The Gradient Descent will work much faster.

# Feature Scaling Method
## Divide by maximum
if $x_1 \in [300, 2000]$, We can scale it by dividing by $2000$ 
so $x_1 \in [0.15, 1]$
## Mean Normalization
We re-scale the features so they range around $0$, and ranges from $[-1,1]$
$$x=\frac{x-\mu}{max-min}$$
as $\mu$ is the mean.

*ex:* if $300\leq x\leq 2000$, and the mean is $600$. then the re-scaled $x$ is:
$$\frac{300-600}{2000-300}\leq x' \leq \frac{2000-600}{2000-300}$$
$$-0.18 \leq x' \leq 0.82$$
## Z-Score Normalization
$$x=\frac{x-\mu}{\sigma}$$
as:
- $\mu :$ mean
- $\sigma :$ standard deviation

*ex:* if $300 \leq x \leq 2000$ and $\mu=600$ and $\sigma=450$. Then the re-scaled $x$ is:
$$\frac{300-600}{450} \leq x' \leq \frac{2000-600}{450}$$
$$-.067 \leq x' \leq 3.1$$
# What to Scale
![[Feature Scaling-20240629195616729.png]]It's better that the values range around zero (unlike last example)
# Notes
- When a particular feature has a large range, it makes the 