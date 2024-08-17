The learning curve might look like this
![[Choosing the Learning Rate-20240703104239615.png]]
this means that:
- The learning rate is large
- There is a bug in the code
And to **debug**:
Set a **very small learning** rate and see the result:
- If the curve is decreasing after very iteration, this means that the learning rate was large
- If the curve sometimes increases after an iteration, this means there is a bug in the code
# How to choose a learning rate
![[Choosing the Learning Rate-20240703104716809.png|651]]
Take a range of numbers, like $[0.001, 1]$ and multiply each time by x$3$ (0.001, 0.003, 0.01, 0.03, ...) and plot the results on the learning curve.

Then choose the curve that:
- Decreases **rapidly** 
- Decreases **constantly** 

Off course you will try these learning rates on a small subset of the training set, not all the training set.