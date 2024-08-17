# Coffee Roasting Model
![[Forward Propagation Implementation with Python (coffee roasting model)-20240802150159487.png]]
- We just compute the activation functions manually.
- We assume that we have the trained parameters, but for now you can just use random parameters until you learn how to train them.
# General Implementation
![[Forward Propagation Implementation with Python-20240802151517562.png]]
- all $w$ parameters represented in $W$ as columns.
- `dense()` function will create layers.
	- `w = W[:,j]` will get the $j^{th}$ column from $W$ which is $w_j^{[l]}$.
- `sqeuntial()` function will link the layers together
	- `f_x` will be the last prediction that we apply the threshold on it.