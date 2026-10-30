# THE NOTEBOOK IS CONNECTED TO COLAB GPU

# What is scalar?
its a single numerical number (0-Dimensional tensor)

# Vector?
is a single dimension tensor that contains many numbers   
so based on that the `vector.ndim` will equal to 1 
keep in mind that n - dim is 1 but the **shape** is the num of numbers the vector has

# Matrix?
okay so this is a 2-dimension tensor
`matrix.ndim` = 2 & `matrix.shape` = num of rows , now to columns
and so u can access each vector of it `matrix[1]` and so on 

# What is a Tensor?
A Tensor is a generalization of scalars, vectors, and matrices to N dimensions.
so 3D Tensor is stack of matrices & 4D Tensor is stack of 3D tensors and so on ..
and the `tensor.ndim`= num of tensors and the `tensor.ndim` = num of tensor + shape of rest (vector , matrix , ten)

**keep in mind**
![alt text](image.png)

## Filling Tensors:
so we can fill tensors as NumPy random numbers by `torch.rand` 
or zeros `torch.zeros` or `torch.ones`
or by range (which creates list of numbers from start to end-1 , if u don't put the start it started auto from zero & also u can add step condition) by `torch.arange` 
We can match shapes with (_like) `torch.zeros_like(input = )`,`torch.ones_like`, `rand_like` 

## Notes
**The default Datatype in tensor is `float_32` unless u specified it and u can change dtype by `tensor.type(new_dtype)`**
**1 - We can specify also the right device to run the tensors(CPU, GPU)**
**2 - be careful Torch does not allow operations between tensors on different devices directly,So move one to anther with `tensor.to('cpu')` this will move the tensor into the CPU device**
**3 - `requires_grad = True` is to track the gradient for backward propagation**


# keep in mind most of tensor errors are :
**Wrong Data type** 
**Wrong Tensor shape**
**Wrong Devices**


