# Activities

## Task 1

Refer to the following link. Discuss how the Recursive Fibonacci with Memoization works:
https://www.cs.usfca.edu/~galles/visualization/DPFib.html
//
The Recursive Fibonacci with Memoization works by storing the results of previously calculated Fibonacci numbers in an array, so that they do not have to be recalculated each time they are needed. This is done to avoid redundant calculations and to improve the efficiency of the algorithm.

The memoization technique works by checking if the value of the nth Fibonacci number has already been calculated and stored in the array. If it has, the stored value is returned. If not, the function recursively calculates the nth Fibonacci number using the formula F(n) = F(n-1) + F(n-2), and stores the result in the array before returning it.

The use of memoization significantly improves the efficiency of the algorithm, especially for larger values of n, by reducing the number of recursive calls needed and eliminating redundant calculations.

## Task 2

The stair case problem can be solved based on the Fibonacci series. There is a simple implementations in `./src/staircase2.cpp`.

- Explain how the code works. The following link might be useful:
  https://dev.to/alisabaj/the-climbing-staircase-problem-how-to-solve-it-and-why-the-fibonacci-numbers-are-relevant-3c4o

  // The given code defines two functions fib() and countWays(). fib() is a recursive function that returns the n-th Fibonacci number by adding the two previous numbers in the sequence. countWays() calls fib() with argument s+1 to calculate the number of ways to reach the s-th stair, assuming that the person can climb either 1 or 2 stairs at a time. The program then prints the result using cout.

- Modify the code to use Dynamic Programming (Memoization)

```c++
#include <iostream>
using namespace std;

// Memoization array to store previously calculated Fibonacci numbers
int memo[100];

// A dynamic programming function to
// find N'th fibonacci number
int fib(int n)
{
    if (memo[n] != -1)
        return memo[n];
    if (n <= 1)
        memo[n] = n;
    else
        memo[n] = fib(n - 1) + fib(n - 2);
    return memo[n];
}

// Returns number of ways to reach s'th stair
int countWays(int s)
{
    // Initializing memo array with -1
    for (int i = 0; i < 100; i++)
        memo[i] = -1;
    return fib(s + 1);
}

// Driver C
int main()
{
    int s = 4;

    cout << "Number of ways = " << countWays(s);

    return 0;
}

```
## Task 3

Explain how the code in `./src/staircase3.cpp` works.

// This program uses dynamic programming and the Fibonacci sequence to calculate the number of ways to reach the nth stair in a staircase.

The fib() function is a recursive implementation of the Fibonacci sequence, with an additional dp array parameter to store previously computed values. If the dp array already contains a value for n, it simply returns the value. Otherwise, it calculates the nth Fibonacci number and stores it in the dp array before returning the result.

The countWays() function initializes a dp array with -1 values, calls the fib() function to calculate the nth Fibonacci number, and returns the value of dp[n].

The main function initializes the variable n to 4 and prints the number of ways to reach the 4th stair using the countWays() function.

Overall, the program demonstrates an efficient way to solve a problem using dynamic programming and the recursive Fibonacci sequence implementation.

## Task 4: Individual (at home)

- There are `n` stairs, a person standing at the bottom wants to reach the top. Write a program that counts the number of ways someone can climb up to m stairs for a given value m. For example, if m is 4, it is possible to climb 1 stair or 2 stairs or 3 stairs or 4 stairs at a time. Make sure you use. Refer to the link below:
  https://www.geeksforgeeks.org/count-ways-reach-nth-stair/
  
```c++

#include <iostream>
using namespace std;

// Function to count the number of ways to reach m stairs
int countWays(int n, int m)
{
    int dp[n + 1];
    dp[0] = 1;
    for (int i = 1; i <= n; i++)
    {
        dp[i] = 0;
        for (int j = 1; j <= m && j <= i; j++)
        {
            dp[i] += dp[i - j];
        }
    }
    return dp[n];
}

// Driver code
int main()
{
    int n = 4;
    int m = 3;
    cout << "Number of ways to reach " << n << " stairs with maximum " << m << " steps at a time = " << countWays(n, m) << endl;
    return 0;
} 

```
## Links

- https://cpp.sh/
- [leetcode.com](https://leetcode.com/problems/climbing-stairs/)
