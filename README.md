# NORMALIZATION PROBLEM

import numpy as np

#Making an 5x5 array with random values inside the variable X

X = np.random.random((5,5))

#Finding the square root of each values in the array X

f = np.std(X)

#Finding the mean of all the values inside the array

v = np.mean(X)

#Formula for Normalization, used on each value in the array

z = (X - v) / f

#Print the final values after the Normalization solution

z

#save array Z using the file name X_normalized.npy and printing that its succesfully saved

np.save('X_normalized.npy', z)

print ("\nThe work has been saved at 'X_normalized.npy' ")


# DIVISIBLE BY 3 PROBLEM

import numpy as np

#Making an Array with the values 1 to 100 inside the variable ndarray

ndarray = np.arange(1,101,1)

#Organizing the array by 10x10 in ascending order

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

#save array using the file name div_by_3.npy and printing that it is saved. 

np.save('div_by_3.npy', e)

print ("\nThe work has been saved at 'div_by_3.npy' ")
