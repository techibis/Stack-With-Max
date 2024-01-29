Extending stack interface
View PDF at this link: https://awstechu.instructure.com/courses/516/files/66828?wrap=1
**Problem Introduction
Stack is an abstract data type supporting the operations Push() and Pop(). It is not difficult to implement it in a way that both these operations work in constant time. In this problem, you goal will be to implement a stack that also supports finding the maximum value and to ensure that all operations still work in constant time.
**Problem Description
Task. Implement a stack supporting the operations Push(), Pop(), and Max().
Input Format. The first line of the input contains the number 𝑞 of queries. Each of the following 𝑞 lines
specifies a query of one of the following formats: push v, pop, or max.
Constraints. 1 ≤ 𝑞 ≤ 400000, 0 ≤ 𝑣 ≤ 105.
Output Format. For each max query, output (on a separate line) the maximum value of the stack.
**Time Limits.
language C C++ Java Python C# Haskell JavaScript Ruby Scala time(sec)111.551.52 5 53
Memory Limit. 512MB. Sample 1.

Explanation:
After the first two push queries, the stack contains elements 1 and 2. After the pop query, the element 1 is removed.
Sample 2.   
5
push 2 push 1 max pop max
 2 2
5
push 1 push 2 max pop max
 2 1
12
Sample 3.
Input:
 10 push 2 push 3 push 9 push 7 push 2 max max max pop max
Output:
Sample 4.
Input:
Output: Explanation:
The output is empty since there are no max queries. Sample 5.
Input:
Output:
Starter Files
The starter solutions in C++, Java, and Python3 process the queries naively: for each max query they scan the current contents of the stack to find the maximum value. Hence the max query has running time proportional to the size of the stack. Your goal is to modify it so that its running time becomes constant. For other programming languages, you need to implement a solution from scratch.
 9 9 9 9
 3
push 1 push 7 pop
  6
push 7 push 1 push 7 max pop max
 7 7
13

What to Do
Think about using an auxiliary stack.
