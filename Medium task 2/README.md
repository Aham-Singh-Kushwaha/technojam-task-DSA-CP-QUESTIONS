Although this program felt simple, but it was rather tricky. I faced many **issues** during this program , the first one being the leetcode compiler giving me Time-Limit exceeded error. So i had to resort to a faster algorithm rather than simply checking for a number's predecessor for prime.
The second one being that the compiler passed all the test cases , but when i tried to submit it gave me a wrong answer message. But i succeded in the end.


1. count = 0
    For i from 1 to n-1 do
        if isPrime(i) then count = count + 1
    return count
2. To check for prime:
      if n == 0 or n == 1 return false
    if n == 2 return true
    For i from 2 to sqrt(n) do
        if n % i == 0 then return false
    return true
    
    **This code is correct in all ways, but this still gives random errors on leetcode, like time-limit exceeded and wrong answer error. So we have to improvise and use a better bottom-up approach on this problem.**
    
    
    count = 0
    notPrime = a boolean array with n slots, initially all false
    For i from 2 to n do
        if !notPrime[i] then
            count = count + 1
            For j from 2 to k where k * i < n do
                notPrime[i * j] = true
    return count
 
 We have an array to check for prime which is initially false and turns true if any number matches the prime conditions,i.e. the factor count method.
