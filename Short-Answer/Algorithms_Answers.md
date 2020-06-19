#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  The while loop is written in n^3 but a is being increased by a sum of n^2.  It would be n^3/(a+n^2), which equals out to O(n).

b)  The for loop is O(n) and the while doubles j every time so j will approach n quicker, therefore it has an O(log n).  When you put them together it will be O(n log n).


c)  The recursive function has a constant time for the base but the recursive call dominates the runtime of the function.  Since it increases in proportion, the final runtime i O(n).


## Exercise II

Another way to rephrase this problem is to guess the value of an unknown number between 0 and n. After each guess, information will be provided whether the unknown number is actually higher or lower than the guess. If the egg breaks, then the guess was too high. If the egg doesn't break, the guess was too low.

A binary search with a runtime of O(log n) should be used to minimize egg breakage. By repeatedly guessing the midpoint of the current working range, half of the possibilities will be eliminated on each turn. If the egg breaks, choose the lower half and if the egg doesn't break, choose the upper half. The solution is found when the current working range is so small that it can be seen that an egg doesn't break on floor f but breaks on floor (f - 1).
