# Activities

## Task 1

- Refer to the following link. Discuss how the
  Recursive Factorial works:
  https://www.cs.usfca.edu/~galles/visualization/RecFact.html

  //The Recursive Factorial function uses recursion to repeatedly call itself with decreasing values of "n" until it reaches a base case of 0 or 1, where it returns 1. It then multiplies the current value of "n" with the returned value from the previous level and continues this process until the initial call is reached, and the final result is returned as the factorial of the input number "n". The provided visualization demonstrates this process step by step.  

- Refer to the following link. Discuss how the Recursive Fibonacci works:
  https://www.cs.usfca.edu/~galles/visualization/DPFib.html

  //The Recursive Fibonacci function computes the nth Fibonacci number by recursively calling itself with decreasing values of "n" until it reaches base cases of 0 or 1, then returning the value of "n". For other cases, it recursively calls itself with the values of "n-1" and "n-2" and returns the sum of the results. The provided visualization demonstrates this process step by step and highlights the computational expense of this approach for larger values of "n".

## Task 2

There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs at a time. There is a simple implementations in `./src/` folder. Discuss how the code works.

//

 The code implements a recursive function called number_of_paths(n) that calculates the number of distinct ways a person can climb a staircase with n stairs. The function uses the following base cases:

If n is less than or equal to 0, there are no ways to climb the staircase, so the function returns 0.
If n is equal to 1, there is only one way to climb the staircase (by taking one step), so the function returns 1.
If n is equal to 2, there are two ways to climb the staircase (by taking one step twice or by taking two steps at once), so the function returns 2.
For any other value of n, the function recursively calls itself with the values of n-1 and n-2, representing the number of ways to climb the remaining stairs if the person takes one or two steps on the first move. The function then returns the sum of the results of these recursive calls, representing the total number of ways to climb the entire staircase.

In the main() function, the number_of_paths(n) function is called with an input value of 4, and the result is printed to the console using cout. This should output "number of paths = 5", indicating that there are five distinct ways to climb a staircase with 4 stairs.

## Task 3

- There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs or **3 stairs** at a time. Write a program that counts the number of ways, the person can reach the top. You can use the following program as a starter `./src/staircase1.cpp`. Also the link below might useful:
  https://www.includehelp.com/cpp-programs/stair-case-program-to-solve-the-staircase-problem.aspx

```c++
#include <iostream>
using namespace std;

int number_of_paths(int n)
{
    if (n <= 0)
        return 0;
    if (n == 1)
        return 1;
    if (n == 2)
        return 2;
    if (n == 3)
        return 4; // 1+1+1, 1+2, 2+1, 3

    return number_of_paths(n - 1) + number_of_paths(n - 2) + number_of_paths(n - 3);
}

int main()
{

    cout << "number of paths =  " << number_of_paths(4);
    return 0;
}
```
## Task 4: Individual (at home)

- What are the pros/cons of recursive over iterative Programming?

// Recursive programming is often simpler and more elegant for certain problems, but it can be slower and less memory-efficient for large-scale problems. It can also be harder to optimize and debug. Iterative programming is often faster and more memory-efficient, but it can be more complex and less intuitive. It is better suited for more complex problems and for parallel computing. The choice between recursive and iterative programming depends on the specific problem and the needs of the program.

- Difference between recursion and induction.

// Recursion and induction are both methods of mathematical reasoning, but they are used in different contexts.

Recursion is a programming technique where a function calls itself to solve a problem. It is used in computer science to break down a problem into smaller subproblems that are easier to solve, until the base case is reached. Recursion is a useful tool for solving problems where the solution depends on smaller instances of the same problem.

Induction is a mathematical proof technique that is used to prove a statement for all natural numbers. It consists of two steps: the base case, where the statement is shown to hold for the smallest value of n, and the induction step, where it is shown that if the statement holds for n, then it also holds for n+1. Induction is used to prove statements about sequences, series, and other mathematical structures.

In summary, recursion is a programming technique for breaking down a problem into smaller subproblems, while induction is a mathematical proof technique for proving statements about all natural numbers.

> Refer to the [links](#links) section below.

## Links

- https://cpp.sh/
- [Difference Between Recursion and Induction](https://www.geeksforgeeks.org/difference-between-recursion-and-induction/)
- [Recursion vs Iterative Programming](https://www.softwaretestinghelp.com/recursion-in-cpp/)
