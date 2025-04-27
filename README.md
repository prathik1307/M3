# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float rate, int months) {
float monthlyRate = rate / (12 * 100);
float emi;
emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) / (pow(1 + monthlyRate, months) - 1);
printf("Monthly EMI: %.2f\n", emi);
}
int main() {
float principal, rate;
int months;
printf("Enter principal amount: ");
scanf("%f", &principal);
printf("Enter annual rate of interest (in percentage): ");
scanf("%f", &rate);
printf("Enter number of months: ");
scanf("%d", &months);
calculateEMI(principal, rate, months);
return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/b1dafae1-ccb1-40e3-8585-565004153ca8)




## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
int n = 6, first = 0, second = 1, next;
printf("Fibonacci series for %d terms:\n", n);
printf("%d %d ", first, second);
for (int i = 2; i < n; i++) {
next = first + second;
printf("%d ", next);
first = second;
second = next;
}
printf("\n");
return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/67acbe8f-d283-4a59-890d-545d7cf1d159)






## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
int n;
printf("Enter the number of elements: ");
scanf("%d", &n);

int arr[n];
printf("Enter %d elements:\n", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
}
printf("The last element of the array is: %d\n", arr[n - 1]);
return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/ca7e512f-efe5-4f26-823b-64a96ccf55a9)







## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
int n, count = 0;
printf("Enter the number of elements: ");
scanf("%d", &n);
int arr[n];
printf("Enter %d elements:\n", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);
if (arr[i] > 0)
{
count++;
}
}
printf("Total number of positive elements: %d\n", count);
return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/fa4f014e-e3c6-466e-8487-2c735982bfd1)




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
int main() {
int n;
printf("Enter the number of elements: ");
scanf("%d", &n);
int arr[n];
printf("Enter %d elements:\n", n);
for (int i = 0; i < n; i++) {
scanf("%d", &arr[i]);

}
printf("Updated array:\n");
for (int i = 0; i < n; i++) {
if (arr[i] % 2 == 0) {
printf("E ");
} else {
printf("%d ", arr[i]);
}
}
printf("\n");
return 0;
}
```
## Output:
 
![image](https://github.com/user-attachments/assets/0190988e-25aa-4d0e-87f1-4de08d76fc3c)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



