![[Build a Neural Network-20240802101310125.png]]
- What we saw earlier was an **explicit** way to create layers and implement **Forward Propagation**.
![[Build a Neural Network-20240802104737733.png]]
- Instead of passing the value to the layers manually, we just create the layers and use the last 3 lines of code to train and predict.
- `Sequential()` Links the layers given to it in order. And do what we did by passing the values from and to each layer.
- Instead of assigning each layer to a variable, we just define them at once in the `Sequential()` Function
  ![[Build a Neural Network-20240802105105246.png|426]]
  And this is the **Digit Classification** example code:
  ![[Build a Neural Network-20240802105343029.png]]