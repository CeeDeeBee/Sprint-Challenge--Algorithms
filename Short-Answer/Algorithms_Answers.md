#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) This is an example of code with the runtime of O(n). The first line has a complexity of
O(1). The while loop on the second line would be O(n^3) but the counting variable is incrementing by n \* n so the while loop simplifies to a < n which is O(n). The code to increment the counting variable is also O(1). This means the overall complexity is O(1 + 1 + n) which can be simplified to O(n).

b) This code has a runtime of O(n log n). The first, third, fifth, and sixth lines all have a complexity of O(1). The interesting part of the code is the two loops. The outer loop has a complexity of O(n). The inner loop then has the complexity of O(log n) because its counter variable is increasing by 2 on every execution. Because the loops are nested you multiply the runtimes and are left with O(n log n)

c) This code has a runtime of O(n). They key line here is the return statement where the function calls itself with one less "bunny". There is a base case written for when bunnies are zero. This means that the code will run n times where n is the number of bunnies.

## Exercise II

A good strategy here could look just like a binary search of a sorted array. In order to minimize the number of eggs dropped you would want to start at the middle most floor of the building and drop an egg. If the egg does not break you know that all the floors below you can not be f and you can perform the same strategy of taking the middle value of all the floors above you. If the egg does break you can do some simmilar but in reverse. Here you know that f can not be any floor above you or the current floor and you find the middle value of of the floors below and again repeat the process. This process continues until you only have three possible values. You drop at the middle value and if the egg does break you know that f is the floor below you. If the egg does not break you know that f is either the current floor or one above. You then test the floor above and if the egg breaks f is the floor one down. If the egg does not break f is the current floor. This algorithm would have a runtime complexity of O(log n) as it is essentially a binary search which in the worst case has to check half of the values of the given array.
