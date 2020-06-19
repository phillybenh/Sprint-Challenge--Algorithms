#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) This is time complexity of O(n). The while loop looks like it could be n^3, but since a is updated with a+ n^2, i think some of that cancells it out.

b) Time complexity of O(n log n). Normally I'd assume nested loops are O(n^2), but since the inner loop increments with j*=2 it is O(log n). Ultimately giving this time complexity of O(n) * O(log n) = O(n log n).

c) This has a runtime complecity of O(n). As n increases, the number of recursion cycles increases linearly.

## Exercise II
There are a couple ways to do this, but since we're supposed to minimize the number of `dropped+broked` eggs adn floors are inherently sorted, we will do this similarly to a binary search.

In plain English:
1. Drop an egg from the middle floor of the floors being considered.
2. Did it break? Yes or no.
3. 
    3a. If yes, eliminate the upper floors from our consideration and proceed to step 4.
    3b. If no, eliminate the lower floors form our consideration and proceed to step 4. 
4. Restart the process with step 1 until we reach our answer.

Runtime complexity of this solution is O(log n)


