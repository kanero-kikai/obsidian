Let's see how to predict using Neural Networks.
![[Pasted image 20240801142541.png]]
- This is a handwritten digit recognition application. We will predict only two digits: 0, 1.
- The digits are 8x8 pixels. So we can represent them is a 8x8 Matrix.
- 0 -> Black, 255 -> White.
- 
- The network has 2 Hidden layers: One with 25 hidden units, and the other with 15 hidden units. And the output layer has 1 unit.
- 
- $\vec a ^ {[1]}$ is computed with $25$ activation functions of the input vector $\vec x / a^{[0]}$ as shown in the image.
- And then $\vec a ^{[2]}$ is computed with $15$ activation functions of $\vec a ^ {[1]}$ 
  ![[Pasted image 20240801143314.png|345]]
- And then $a^{[3]}$ is computed with $1$ activation function of $\vec a ^ {[2]}$, and the last Sigmoid function is applied to get the final prediction $f(x)$
  ![[Inference (Making Predictions) - Forward Propagation-20240801143823496.png|325]]

And this is the forward propagation algorithm, going forward from left to right.
$\vec{x}$ -> $\vec{a}^{[1]}$ -> $\vec{a}^{[2]}$ -> $a^{[3]}$
![[Inference (Making Predictions) - Forward Propagation-20240801144116976.png]]