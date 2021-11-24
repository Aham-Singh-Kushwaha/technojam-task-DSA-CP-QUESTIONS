For example, a ^ b = c, where c is given, and the first element(a) is also given. If we do a ^ c then we will get b, our second element in the output array.
We do the above mentioned our code and this gives us the original array.

1.Find the array's length.
2.Create a new array of size one more than the encoded one.
3.Store the "first" element at 0 index of new array.
4.For from i=0 to i<length of array.
5.Store new array[index i] XOR encoded array[index i] at new array index i+1.
6.Return the new array.                           
                           
