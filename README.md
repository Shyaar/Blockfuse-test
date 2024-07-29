# Blockfuse-test (question 1)
Fuzz data:
[76, 57, 19, 87, 62, 23, 87] 
[57, 10, 2, 40, 40, 35, 36, 59, 43, 7, 98, 90, 33, 11] 
[67, 47, 63, 40, 29, 65, 100, 7, 69, 57, 59, 36, 68, 33, 16] 
[7, 10, 45, 21, 71, 27, 97, 73, 25] 

Approach 1

Given that we have been provided with 4 arrays to find the median of two sorted arrays (nums 1 and nums 2) i take that the first 2 arrays combined = nums 1 and the last 2 arrays = nums 2.

Solutions:
nums 1:
Sorted array 1: (19, 23, 57, 57, 62, 76, 87, 87)
sorted array 2: (2, 7, 10, 11, 33, 35, 36, 40, 40, 43, 59, 90, 98)
Combined (array 1 and 2) : (2, 7, 10, 11, 19, 23, 33, 35, 36, 40, 40, 43, 57, 57, 59, 62, 76, 87, 87, 90, 98) 

There are 21 Total Elements: which give a value that is odd, so the median is the middle element: which is 40
hence nums 1 = 40

Nums 2:

sorted array 1: (7, 16, 29, 33, 36, 40, 47, 57, 59, 63, 65, 68, 69, 100)
Sorted array 2: (7, 10, 21, 25, 27, 45, 71, 73)

Combined (array 1 and 2): Combined (7, 10, 16, 21, 25, 27, 29, 33, 36, 40, 45, 47, 57, 59, 63, 65, 68, 69, 71, 73, 97, 100)

There are 22 Total Elements: which give a value that is even, so the median is the summation of the 2 middle element divided by 2: which is 47+47/2, 45+47= 92, 92/2 = 46

hence nums 2= 46


Approach 2

Take a combination of elements in the provided arrays : (2, 7, 7, 7, 10, 10, 11, 16, 19, 21, 23, 25, 27, 29, 33, 33, 35, 36, 36, 40, 40, 40, 43, 45, 47, 57, 57, 59, 59, 62, 63, 65, 68, 69, 71, 73, 76, 87, 87, 90, 97, 98, 100)

There are 43 Total Elements: which give a value that is odd, so the median is the middle element: which is 40: 
hence the median of the combined arrays is = 40:


