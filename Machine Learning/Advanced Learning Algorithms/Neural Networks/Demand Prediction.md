![[Pasted image 20240725094618.png]]
- **Demand Prediction :** is when we trying to predict if some product will be a top seller
- The **Neuron** takes **input** and do some calculations using **activation function** and gives **output**.
- In this example:
	- **Input :** price.
	- **Activation Function :** Sigmoid function.
	- **Output :** probability of being top seller.
![[Pasted image 20240726205848.png]]
- This is a more advanced neural network.
- The **probability of being a top seller** depends on some factors (affordability, awareness, perceived quality). And we get those factors from the values in the **input layer**.
- **A Layer** is a group of **Neurons**, or **One Neuron**
-  It consists of:
	- **Input Layer**
		- It's the layer on the left which has the **features**.
	- **Hidden Layer**
		- It takes the values from Input Layer and do some calculation (affordability, awareness, perceived quality -> **Activations**) 
	- **Output Layer**
		- It takes the values from the **Hidden Layer** and do the final prediction
		- the **probability of being a top seller** is the **activation** for the **Output Layer**
- **How it works:**
	- The network takes the values from the **Input Layer** and do some calculations (**Activations**) to compute some factors which the final result depends on.
		- The **Output Layer** takes the values of those factors and compute the final result.
## Understand Neural Network
![[Pasted image 20240726212004.png]]
- Remember **Feature Engineering**, When we get better feature that gives better prediction from the existing features? This is what the **Neural Network** do. **It creates better and more predictive feature from existing features.** But unlike feature engineering where you need to create feature yourself, **the neural network does it by itself**.
- The values moves from layer to another as **vectors**  $\vec{x}$ -> $\vec a$ -> $a$ 
  Input layer -> hidden layer -> output layer.
## Multiple Hidden Layers
![[Pasted image 20240726222315.png]]
Neural networks usually have more than 1 hidden layer.
  