#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) This is an example of code with the runtime of O(n). The first line has a complexity of
O(1). The while loop on the second line would be O(n^3) but the counting variable is incrementing by n \* n so the while loop simplifies to a < n which is O(n). The code to increment the counting variable is also O(1). This means the overall complexity is O(1 + 1 + n) which can be simplified to O(n).

b) This code has a runtime of O(n log n). The first, third, fifth, and sixth lines all have a complexity of O(1). The interesting part of the code is the two loops. The outer loop has a complexity of O(n). The inner loop then has the complexity of O(log n) because its counter variable is doubling on every execution. Because the loops are nested you multiply the runtimes and are left with O(n log n)

c) This code has a runtime of O(n). They key line here is the return statement where the function calls itself with one less "bunny". There is a base case written for when bunnies are zero. This means that the code will run n times where n is the number of bunnies.

## Exercise II

A good strategy here could look just like a binary search of a sorted array. In order to minimize the number of eggs dropped you would want to start at the middle most floor of the building and drop an egg. If the egg does not break you know that all the floors below you can not be f and you can perform the same strategy of taking the middle value of all the floors above you. If the egg does break you can do something similar but in reverse. Here you know that f can not be any floor above you and you find the middle value of of the floors below, including the current floor, and again repeat the process. This process continues until you only have two possible values. If there is one value that is f. If there are two you go to the lower floor and drop the egg. If it breaks then the current floor is f. If it doesn't break, the floor above is f. This algorithm would have a runtime complexity of O(log n) as it is essentially a binary search which in the worst case has to check log2(floors) times.
