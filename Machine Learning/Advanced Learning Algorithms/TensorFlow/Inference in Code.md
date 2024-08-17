We gonna learn how to implement neural networks with TensorFlow.
![[Inference in Code-20240801205857039.png|505]]
- The example we are using is coffee roasting example.
- We roast raw coffee beans to get good coffee.
- We want to predict weather the coffee beans with features in vector $\vec x$ is a good coffee or not.
![[Inference in Code-20240801210254597.png|509]]
- We create an array **x** with the data. (Notice that it's a matrix not a vector [[Data in TensorFlow]])
- We create the first layer **layer_1**
	- The layer type is **Dense**, and this is the layer we learned about earlier.
	- **units** is the number of **hidden units**
	- **activation** is the type for the **activation function**
- Then we get the **first output vector** $\vec{a}^{[1]}$ by passing **x** to **layer_1**
![[Inference in Code-20240801210745803.png]]
- For the output layer **layer_2**, we create a **Dense** layer with 1 **unit**.
- Then we apply **layer_2** function to the **a1** vector.
![[Inference in Code-20240801210906139.png|247]]
- Then we apply the threshold to get the final prediction.
## Handwritten digit recognition code
[[Inference (Making Predictions) - Forward Propagation]]
![[Inference in Code-20240801211128657.png]]