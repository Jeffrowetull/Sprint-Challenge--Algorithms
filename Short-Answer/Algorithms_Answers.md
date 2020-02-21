#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)reduced down, it is O(3n) which is O(n)


b)The for loop lasts as long as range(n) so it's O(n)


c)Another linear function. It is O(n) because it can only recursively call bunnyEars "bunnies" amount of times

## Exercise II

Binary search would be a great candidate for finding out which floor eggs break at, but it would need one small change. To actually know whether the floor is the one, you would have to compare it to either the preceding or succeeding floor depending on the egg's fate. 

For instance, we test the middle floor and the egg doesn't shatter. The middle floor cannot be floor f until it is known that it breaks on the next floor. So you would check the next floor as well. If the egg does break, check the preceding floor before recursing on the earlier half.

This would give the equation O(n+log(n)) complexity but I think it would be shorter than normal binary search and not wasting too many eggs because you're actually testing each floor.


