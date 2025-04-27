# EX3 Implementation of Tower of Hanoi
## DATE : 26.04.2025
## AIM :
To write a C program to implement Tower of Hanoi

## Algorithm
1.Start the program.
2.If n > 0, continue with the following steps.
3.Recursively move n-1 disks from the source rod (x) to the auxiliary rod (z) using the destination rod (y) as helper.
4.Print the move of the nth disk from the source rod (x) to the destination rod (y).
5.Recursively move the n-1 disks from the auxiliary rod (z) to the destination rod (y) using the source rod (x) as helper.
6.Initially call the function as TOH(n, 'A', 'B', 'C'), where 'A', 'B', and 'C' are the rod names.
7.End the program.

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: vinodhini k
RegisterNumber: 212223230245
*/

#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
if(n>0)
{
TOH(n-1,x,z,y);
printf("%c to %c",x,y);
printf("\n");
TOH(n-1,z,y,x);
}
}
int main()
{
int n=2;
TOH(n,'A','B','C');
}
```

## Output:

![image](https://github.com/user-attachments/assets/2f34179f-ac64-4f00-8bb5-c9947c010e7c)


## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
