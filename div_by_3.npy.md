import numpy as np

# Making an Array with the values 1 to 100 inside the variable ndarray
ndarray = np.arange(1,101,1)

# Organizing the array by 10x10 in ascending order
c = ndarray.reshape(10, 10)

#Squaring all numbers in the array
d = np.square(c)

#Storing all elements that are divisible by 3 at variable e
e = d[d % 3 == 0]

#Printing the variable c which contains the values 1 to 100 in an 10x10 array
print (c)

#Space for asthethic 
print ()

#Printing the variable e which contains all values divisible by 3
print (e)

#save array using the file name div_by_3.npy
np.save('div_by_3.npy', e)
