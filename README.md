
# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>
int main() {
int M, N;
scanf("%d %d", &M, &N);
int start = (M > N) ? M : N;
int end = (M < N) ? M : N;
if (start % 2 != 0) {
start--;
for (int i = start; i >= end; i -= 2) {
printf("%d ", i);
}
return 0;
}

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/e822f72f-3c58-465e-87f5-97fccf5240f1)











## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>
int main() {
int rows, i, j;
printf("Enter the number of rows: ");
scanf("%d", &rows);
for (i = 1; i <= rows; i++) {
for (j = 1; j <= i; j++) {
printf("* ");
}
printf("\n");
}
return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/4930b0c9-939b-4155-9c82-faaf472d410f)






## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include<stdio.h>
int addition(int a,int b)
{
return a+b;
}
int substraction(int a,int b)
{
return a-b;
}
int main()
{
int a,b;
scanf("%d%d",&a,&b);
int result_addition=addition(a,b);
int result_substraction=substraction(a,b);
printf("Addition: %d\n",result_addition);
printf("Subtraction: %d",result_substraction);
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/93698d01-4c90-4749-8a1a-3290be6e9fc5)






## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main() {
int num, sum = 0, digit;
printf("Enter a number: ");
scanf("%d", &num);
for (; num != 0; num /= 10) {
digit = num % 10;
if (digit % 2 != 0) {
sum += digit;
}
}
printf("Sum of odd digits = %d\n", sum);
return 0;
}

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/58730db7-c324-4a1f-8489-16e83624b205)




## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
void fact() {
int N, i;
unsigned long long fact = 1;
printf("Enter a number: ");
scanf("%d", &N);
for (i = 1; i <= N; i++) {
fact *= i;
}
printf("Factorial of %d is %llu\n", N, fact);
}
int main() {
fact();
return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ceba0a1a-b615-4840-ac25-7c2ad92da66c)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
