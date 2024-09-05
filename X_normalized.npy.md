#2ECEB_Santos-PA2

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

#save array Z using the file name X_normalized.npy
np.save('X_normalized.npy', z)
