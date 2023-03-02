# Activities

## Task 1

Refer to the following link. Explain how the Knapsack Algorithm works:
https://monicagranbois.com/knapsack-algorithm-visualization/

// The Knapsack Algorithm is a problem-solving approach used in computer science to maximize the value of items packed in a knapsack while not exceeding a given weight capacity. It works by identifying the most valuable items that can be added to the knapsack without exceeding its weight capacity, and it does this by sorting the items by their value-to-weight ratio and iterating through the list of items to select the ones that can be added to the knapsack. The algorithm is a useful tool for solving optimization problems where a limited amount of resources must be allocated in the most effective way possible.

## Task 2

Refer to the following link. What are the difference between the brute force and the optimized solutions to the Knapsack problem.
https://www.educative.io/blog/0-1-knapsack-problem-dynamic-solution

// The Knapsack problem is an optimization problem that seeks to maximize the value of items that can be packed into a knapsack while not exceeding a given weight capacity. The brute-force approach involves enumerating all possible combinations of items, which can be computationally expensive, particularly when the number of items is large. The optimized solution, such as dynamic programming, breaks the problem down into smaller sub-problems and reuses previously solved solutions, which can be more efficient than the brute-force approach. The main difference between the brute-force and optimized solutions to the Knapsack problem is their computational complexity and efficiency.

## Task 3

There are different implementations of the stair case problem in the following link:
https://www.enjoyalgorithms.com/blog/climbing-stairs-problem

Compare the time and space complexity of the different approaches

// The staircase problem is a problem-solving approach that involves finding the number of distinct ways to climb a staircase of n steps while taking either 1 or 2 steps at a time. There are different implementations of the staircase problem, including recursive, memoization, and dynamic programming approaches, each with different time and space complexities.

The recursive approach involves breaking the problem down into smaller sub-problems and using recursion to solve them. This approach has a time complexity of O(2^n) and a space complexity of O(n), making it less efficient than the other approaches.

The memoization approach, also known as top-down dynamic programming, involves storing the results of previous computations in a lookup table to avoid redundant computations. This approach has a time complexity of O(n) and a space complexity of O(n), making it more efficient than the recursive approach.

The dynamic programming approach, also known as bottom-up dynamic programming, involves solving the problem by building up solutions to sub-problems iteratively. This approach has a time complexity of O(n) and a space complexity of O(1), making it the most efficient approach among the three.

Overall, the time and space complexity of the different implementations of the staircase problem vary depending on the approach used. The recursive approach has a higher time complexity than the memoization and dynamic programming approaches, while the dynamic programming approach has the lowest space complexity among the three. Therefore, the dynamic programming approach is considered the most efficient approach to solving the staircase problem.

## Task 4: Individual (at home)

- Difference between divide and conquer and dynamic programming

// Divide and conquer and dynamic programming are both problem-solving techniques used in computer science. Divide and conquer involves breaking down a complex problem into smaller sub-problems and solving each sub-problem independently, while dynamic programming involves solving a problem by breaking it down into smaller sub-problems and storing the solutions to these sub-problems in a table. Divide and conquer is recursive in nature and is well-suited for problems that can be easily divided into smaller sub-problems, while dynamic programming is more efficient due to the reuse of previously solved sub-problems. Overall, the two approaches differ in their approach to solving problems and their efficiency in terms of time complexity.


- State some application of dynamic programming

// Dynamic programming is a problem-solving technique that has various applications in computer science and beyond. It is commonly used for optimization problems, path-finding algorithms, image and signal processing, bioinformatics, and artificial intelligence and machine learning. Dynamic programming involves breaking down a complex problem into smaller sub-problems and storing the solutions to these sub-problems in a table to avoid redundant computations. This approach reuses the solutions to previously solved sub-problems to solve the original problem more efficiently. Dynamic programming is a versatile and efficient technique used to solve a wide range of problems in various fields.

- Difference between recursion vs dynamic programming

// Recursion and dynamic programming are two problem-solving techniques used in computer science. Recursion is a technique where a function calls itself repeatedly until a base case is reached. Dynamic programming involves breaking down a problem into smaller sub-problems and storing the solutions to these sub-problems in a table. Recursion is simpler to implement, but it can be less efficient and may result in redundant computations. Dynamic programming is more efficient, but it requires more memory to store solutions to sub-problems. Both techniques have their strengths and weaknesses and are used in different scenarios depending on the problem at hand.

- Difference between Top down and bottom up approaches to dynamic programming

// Top-down and bottom-up are two approaches to implementing dynamic programming. Top-down involves breaking down a problem into smaller sub-problems recursively, starting from the original problem, and storing the solutions to these sub-problems in a table to avoid redundant computations. Bottom-up involves breaking down a problem into smaller sub-problems iteratively, starting from the smallest sub-problems, and working up to the original problem, storing the solutions to these sub-problems in a table. Top-down may be more intuitive and easier to implement, but it can suffer from the overhead of function calls and may have a higher risk of stack overflow. Bottom-up may be more efficient and less prone to stack overflow, but it can be more complex to implement and may require more memory.

- How to solve a Dynamic Programming Problem?

// To solve a dynamic programming problem, follow these steps:

1. Identify the problem: First, identify the problem you want to solve and determine whether it can be solved using dynamic programming.

2. Define the sub-problems: Break down the problem into smaller sub-problems. Define the sub-problems in a way that allows you to reuse solutions to previously solved sub-problems.

3. Formulate a recursive relation: Determine the relationship between the sub-problems and the original problem. Use this relationship to formulate a recursive relation.

4. Create a memoization or tabulation table: Decide whether to use the top-down or bottom-up approach and create a table to store the solutions to the sub-problems.

5. Solve the sub-problems: Solve the sub-problems in the order specified by the approach you chose (top-down or bottom-up).

6. Reconstruct the solution: Once all sub-problems have been solved, reconstruct the solution to the original problem using the solutions to the sub-problems.

7. Analyze the time and space complexity: Finally, analyze the time and space complexity of your solution to ensure that it meets the performance requirements of the problem.

By following these steps, you can effectively solve dynamic programming problems and optimize the performance of your solutions.

> Refer to the [links](#links) section below

## Links

- https://cpp.sh/
- [Recursion vs dynamic programming](https://www.geeksforgeeks.org/introduction-to-dynamic-programming-data-structures-and-algorithm-tutorials/)
- [How to solve a Dynamic Programming Problem ?](https://www.geeksforgeeks.org/solve-dynamic-programming-problem/)
