The width of any container will be the difference between the index of the two lines (i and j), and the height will be whichever of the two sides is the lowest (min(H[i], H[j])).
we can observe that if we start with the lines on the opposite ends and move inward, the only possible time the area could be larger is when the height increases, since the width will continuously get smaller.
Putting together everything, it's clear that we need to make a 2-pointer sliding window solution. We'll start from either end and at each step we'll check the container area, then we'll shift the lower-valued pointer inward. Once the two pointers meet, we know that we must have exhausted all possible containers and we should return our answer (ans).

1.To do this we check the max difference between the x-axis coordinates and the min height from two consecutive values and multiply them.
2.If the resulting area is greater than its previous value, then we store it as the new max area.
3.We check if we have another height which matches the above criteria:
    if yes then we move forward 
    if no then we check for other values of x.
