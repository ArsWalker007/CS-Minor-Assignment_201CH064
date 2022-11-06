# CS-Minor-Assignment OS 
fibonacci series and collatz sequence using operating system concepts

**Collatz sequence**

C program using the fork() system call that generates Collatz sequence in the child process

**Collatz conjecture**

Consider the following operation on an arbitrary positive integer:

If the number is even, divide it by two.
If the number is odd, triple it and add one.
In short apply the following function repeatedly:

![image](https://user-images.githubusercontent.com/99437098/200189146-b40e07fc-21c5-4813-98a3-fe0f2143e60b.png)


The conjecture states that when this algorithm is continually applied, all positive integers will eventually reach 1.

Example: For n = 35

35, 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1

**OS Process concept**

The starting number will be provided from the command line. After calling fork(), the child process shall output the collatz sequence. The parent has to wait for the child process to complete and then exit the program.

The program also performs error checking to verify that a positive integer is passed through command line.

**Fibonacci series**

A multithreaded C program that generates the Fibonacci sequence.


**Fibonacci numbers**

Fibonacci series is formed by consecutive fibonacci numbers, starting from 0 and 1.

The following recurrence relation defines nth fibonacci number:
![image](https://user-images.githubusercontent.com/99437098/200189239-dc2d7cce-b175-4a78-beb7-9de0843dd470.png)

Example: The first 12 Fibonacci numbers are as follows

0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89 ...

**OS Threading concept**

On the command line, the user will enter the number of Fibonacci numbersthat the program is to generate. The program will then create a separate thread that will generate the Fibonacci numbers, placing the sequence in a buffer shared by the threads. When the thread finishes execution, the parent thread will output the sequence generated by the child thread. Then the parent thread shall wait until the completion of the fibonacci thread and then output the fibonacci series.

