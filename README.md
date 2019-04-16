# Ternary-Search



Ternary search is a divide and conquer algorithm that can be used to find an element in an array. It is similar to binary search where we divide the array into two parts but in this algorithm. In this, we divide the given array into three parts and determine which has the key (searched element). We can divide the array into three parts by taking mid1 and mid2 which can be calculated as shown below. Initially, l and r will be equal to 0 and n-1 respectively, where n is the length of the array.

mid1 = l + (r-l)/3
mid2 = r – (r-l)/3

Note: Array needs to be sorted to perform ternary search on it.

Steps to perform Ternary Search:

First, we compare the key with the element at mid1. If found equal, we return mid1.
If not, then we compare the key with the element at mid2. If found equal, we return mid2.
If not, then we check whether the key is less than the element at mid1. If yes, then recur to the first part.
If not, then we check whether the key is greater than the element at mid2. If yes, then recur to the third part.
If not, then we recur to the second (middle) part.



Time Complexity:  O(log _3(n)), where n is the size of the array.
