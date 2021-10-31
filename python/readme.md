### Array in Python

Array in python is list of same type numbers. number can be integer, float and ddouble

i : integer : 2 byte
l : long    : 4 byte
f : float   : 4 byte
d : double  : 8 byte


from array import array

nums = array('i', [3, 2, 1])  # Array of integers
nums.append(0)  # Can append to array


