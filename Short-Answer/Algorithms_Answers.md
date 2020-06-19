#### Please add your answers to the **_Analysis of Algorithms_** exercises here.

## Exercise I

a) This loop iterates at n^2 speed from 0 to n^3. Simple division shows that there will be n loops, giving us O(n) complexity

b) This is a nested for loop where the outside iterates over every value linearly (O(n)), but the inner loop moves exponentially (O(logn)). The result is a O(nlogn) time complexity

c) This function will run recursively once for each bunny for a time complexity O(n)

## Exercise II

Assuming this doesn't work like actually dropping eggs off of real buildings and you have no prior information about what fall distance would break an egg, I would start at the exact middle floor and drop an egg to see whether it breaks or not. If it does break, I will go halfway between that floor and the ground to drop an egg again. If it doesn't break, I'll go halfway between that middle floor and the top floor. Continue this process of splitting the range in half until adjacent floors are found where one drop breaks the egg and the one below it does not. This process has O(logn) efficiency, and you can solve the problem with log(f) (base 2) eggs. This pattern does have the downside that it will always take that many eggs, and there is no difference between the best case and the worst case. Going into this problem in real life, I would actually start at the bottom floor and drop an egg and go up a floor each time until it breaks, and this has O(1) efficiency because I know that you can break an egg from waist height on your kitchen floor so you really don't need to be dropping them off buildings, I promise it will break every time
