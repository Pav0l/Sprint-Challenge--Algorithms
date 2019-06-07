Add your answers to the Algorithms exercises here.

## Exercise I

a)
for n = 1, it would run 1 time
for n = 2, it would run 2 times
for n = 5, it would run 5 times
therefore the time complexity of the algorithm is O(n)

b)
three nested for loops with range dependent on n => O(n \* n \* n)
fourth nested loop based on constant range => O(k)
O(n^3 + k) => O(n^3)

c)
recursion with stop condition at n=0 and recursive step of n-1.
so for n = 3, it would run n=(3-1 => 2 => 1 => 0(stop)) => 3 loops.
the algorithm is running a recursive "for" loop in len(n) => O(n)

## Exercise II

**Answer:**
I would first find a floor in the middle (n/2) and drop an egg from that floor and observe if it would break.
If it would break, I can eliminate all floors above this floor as "too high" (more than _f_) and then I would find the middle floor in the remaining floors.
If it would not break, I could eliminate all floors below this floor as "too low" (less than _f_) and then would find the middle floor in the remaining floors.

I would repeat this process until the floor _f_ would be the middle floor.

The runtime complexity of this strategy would be O(n\*log n)
