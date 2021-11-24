To maximise the sum in this case we use a very simple rule of **even and odd**; i.e. odd numbers leave output 1 when divide by 2 and evens leave 0.
So we utilise this ; and to maximise our sum we need **greatest possible number of ones and least possible number of zeroes**.
We do this by shuffling the** odd digits to even positions and vice versa**.

1.We take a list and input elements separated by space, for this we use map() and split().
2.Then we check one by one if the elements in the array are even or odd:
  if even: we increment a odd-position counter
  if odd: we increment a even-position counter
3. Then we divide the odds and evens by two take and find the minimum from odd numbers and even positions and vice versa and sum these values.
4. This sum is the maximum possible sum and hence our result.
