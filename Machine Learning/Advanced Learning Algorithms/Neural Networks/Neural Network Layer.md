- A layer is a group of neurons, or 1 neuron.
- The activation function of each neuron is a **Logistic Regression Function (Sigmoid)**
### Zoom into layers
This example is on the previous [[Demand Prediction]]
![[Pasted image 20240730100740.png]]
- $\vec{x}$ : The input vector from the **Input Layer**
- $\vec{w}^{[i]}_{j}, ~b^{[i]}_{j}$ : The parameters of the $j^{th}$ neuron, in the $i^{th}$ layer.
- $a^{[i]}_{j}$ : The output of the activation function of $j^{th}$ neuron is the $i^{th}$ layer.
- $\vec{a}^{[i]}$ : The output vector of the $i^{th}$ layer. Which is the output of the Sigmoid functions.

***Note:*** Layers are indexed, so the **input layer** **is** **layer 0**, and the **3rd hidden layer** **is layer 2**, and **the output layer is layer *n***, where *n* is the number of all layers (*Not including the input layer, we don't count it*).
***Note:*** The **activation function** here has the input vector $\vec{x}$.
![[Pasted image 20240730102652.png]]
- The same for the output layer.
- The output here $\vec a^{[2]}$ is a scalar because the layer has only 1 neuron. 
- The input of this layer is the output of the previous layer.
![[Pasted image 20240730103123.png]]
- The output of the last layer is a scalar.
- In the last step, we do a final logistic regression to find weather the T-Shirt is a top seller or not.
# More complex neural network
- When we say a network has 4 layers, this means the **hidden layers** and the **output layer**, *the input layer (layer 0) isn't counted.*
- Neurons in the hidden layer called **Hidden Units**.
![[Pasted image 20240801135836.png]]
- Layer 3 take $\vec a^{[2]}$ as input and outputs $\vec a^{[3]}$, So in the activation functions the calculations will be on vector $\vec a^{[2]}$.
## Activation Formula
for $l$ layer, $j$ neuron:
$$a_j^{[l]}=g(\vec w_j^{[l]}.\vec a^{[l-1]}+b_j^{[l]})$$
- The input vector $\vec{x}$ will be $\vec a^{[0]}$
