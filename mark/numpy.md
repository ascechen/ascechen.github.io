### Some experience on numpy 
For matlab user, there is a [NumPy for Matlab users](https://docs.scipy.org/doc/numpy/user/numpy-for-matlab-users.html).
 However, I want to highlight it on my own experience. 
 
 ### Main difference
 - semantics: passing by reference and passing by value
 - be careful about [Mutable vs Immutable Objects in Python](https://medium.com/@meghamohan/mutable-and-immutable-side-of-python-c2145cf72747)
 - In python, if you want to copy an array like in matlab: 
 ```python
 import numpy as np
 a = np.zeros(5)
 b = np.array(a)
 ```
 then you change a, it will not influence b. Do NOT use 
 ```python
 b = a
 ```
