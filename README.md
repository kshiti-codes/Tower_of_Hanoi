# Tower_of_Hanoi

## Explanation
1. Main Method:

Defines the number of disks n and the names of the rods (A, B, and C).
Calls the towerOfHanoi method to solve the problem.

2. towerOfHanoi Method:

This is a recursive method that solves the Tower of Hanoi problem.
Base Case: When there is only one disk (n == 1), move it directly from the source rod (fromRod) to the destination rod (toRod).
Recursive Case: For more than one disk:
Move n-1 disks from the source rod to the auxiliary rod using the destination rod as a temporary holding area.
Move the nth disk from the source rod to the destination rod.
Move the n-1 disks from the auxiliary rod to the destination rod using the source rod as a temporary holding area.

## Complexity Analysis
### Time Complexity
The time complexity of the Tower of Hanoi problem is exponential due to the nature of the recursive solution:

1. Number of Moves:

The number of moves required to solve the Tower of Hanoi problem with n disks is 2^n - 1. This is derived from the recurrence relation T(n) = 2 * T(n-1) + 1.

2. Time Complexity:

The time complexity is O(2^n). This is because each recursive call splits the problem into two subproblems of size n-1 and adds a constant amount of work (moving one disk).

### Space Complexity
The space complexity is determined by the recursion stack:

1. Space Complexity:
The space complexity is O(n) because the maximum depth of the recursion tree is n.
