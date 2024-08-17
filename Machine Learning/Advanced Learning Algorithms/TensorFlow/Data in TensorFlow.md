## How to represent Vectors and Matrices in NumPy
![[Data in TensorFlow-20240802094012914.png|668]]
![[Data in TensorFlow-20240802094433423.png]]
- The first two examples are 2-D **matrices** with one row or column is 1. This is why we use **double square brackets** at the beginning and the end, to represent matrices.
- In the last example there is **1 square bracket** at the beginning and the end. And this represents a **vector**, 1-D array.
- **TensorFlow can't deal with vectors**, so when we want to represent a vector we will represent it as a matrix with one dimension is 1.
- Even **Scalars** are represented as Matrices
  ![[Data in TensorFlow-20240802101042023.png]]
![[Data in TensorFlow-20240802095934480.png]]
- So we represent the data from [[Inference in Code]] example as 2-D matrix, not 1-D vector.
## Notes
- **Tensor** : Just think about it as a matrix
- If you want to convert a Tensor to a NumPy array, use `.numpy()` method
  ![[Data in TensorFlow-20240802100857836.png]]
  