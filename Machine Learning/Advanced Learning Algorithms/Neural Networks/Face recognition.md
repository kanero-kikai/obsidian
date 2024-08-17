### Image representation
![[Pasted image 20240729104730.png]]
- The image is represented by a matrix of pixel intensity values or pixel brightness values (0-255).
- We can again represent the matrix as a vector $\vec{x}$.
### Hidden layers values visualization
![[Pasted image 20240729105338.png]]
- The vector $\vec{x}$ is fed the the hidden layers.
- If we visualized the values from the hidden layers, or what the hidden layers are looking for, we find this:
	- At the first hidden layers we find that it's looking for short lines and edges of the image. for example: the first neuron is looking for a $45 \degree$ line, the second line is looking for a $135 \degree$ line (which are edges for something in the image like the edge of a nose or and eye brow) and so on.
	- In the second hidden layer we find the neurons are looking for more bigger and affecting parts of the face.
	- In the last hidden layers, we find that the neurons are looking for complete faces.
And the same for any image recognition
![[Pasted image 20240729110917.png]]