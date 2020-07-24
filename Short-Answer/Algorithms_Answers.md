#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) This is an example of code with the runtime of O(n). The first line has a complexity of
O(1). The while loop on the second line would be O(n^3) but the counting variable is incrementing by n \* n so the while loop simplifies to a < n which is O(n). The code to increment the counting variable is also O(1). This means the overall complexity is O(1 + 1 + n) which can be simplified to O(n).

b) This code has a runtime of O(n log n). The first, third, fifth, and sixth lines all have a complexity of O(1). The interesting part of the code is the two loops. The outer loop has a complexity of O(n). The inner loop then has the complexity of O(log n) because its counter variable is increasing by 2 on every execution. Because the loops are nested you multiply the runtimes and are left with O(n log n)

c) This code has a runtime of O(n). They key line here is the return statement where the function calls itself with one less "bunny". There is a base case written for when bunnies are zero. This means that the code will run n times where n is the number of bunnies.

## Exercise II
