# PyTorch Tensors and Functions
Welcome to the PyTorch Tensors and Functions README! In this document, we will explore PyTorch tensors and some of its fundamental functions, including rand.

# What are Tensors?
Tensors are the fundamental data structure of PyTorch. They are similar to NumPy arrays but are designed to be used on GPUs for accelerated computing. Tensors can have different dimensions (or ranks), similar to matrices in mathematics.

# Creating Tensors
You can create tensors in PyTorch using various methods. Here are some common ones:

python
Copy code
import torch

# Create an empty tensor
empty_tensor = torch.empty(3, 3)
print("Empty Tensor:")
print(empty_tensor)

# Create a tensor with random values
random_tensor = torch.rand(3, 3)
print("\nRandom Tensor:")
print(random_tensor)

# Create a tensor with zeros
zeros_tensor = torch.zeros(3, 3)
print("\nZeros Tensor:")
print(zeros_tensor)

# Create a tensor with ones
ones_tensor = torch.ones(3, 3)
print("\nOnes Tensor:")
print(ones_tensor)

# Create a tensor from a Python list
list_tensor = torch.tensor([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
print("\nTensor from List:")
print(list_tensor)
The rand Function
The rand function in PyTorch is used to create tensors with random values sampled from a uniform distribution over [0, 1).

Syntax
python
Copy code
torch.rand(*size, out=None, dtype=None, layout=torch.strided, device=None, requires_grad=False)
size (tuple): The shape of the tensor.
out (Tensor, optional): The output tensor.
dtype (torch.dtype, optional): The desired data type of the tensor.
layout (torch.layout, optional): The desired layout of the tensor.
device (torch.device, optional): The desired device for the tensor.
requires_grad (bool, optional): If autograd should record operations on the returned tensor.
Example
python
Copy code
import torch

# Create a 3x3 tensor with random values
random_tensor = torch.rand(3, 3)
print("Random Tensor:")
print(random_tensor)
Output:

lua
Copy code
Random Tensor:
tensor([[0.7917, 0.2079, 0.9333],
        [0.3981, 0.4096, 0.5889],
        [0.5088, 0.8546, 0.4027]])
Conclusion
This README covered the basics of PyTorch tensors and introduced the rand function for generating tensors with random values. Tensors are essential for building and training neural networks in PyTorch. Explore more functions and capabilities of PyTorch tensors to harness the power of deep learning!
