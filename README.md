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


void calculateEMI(float principal, float annualRate, int months) {
    float monthlyRate = annualRate / (12 * 100);
    float emi;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, months)) /
          (pow(1 + monthlyRate, months) - 1);

    printf("Monthly EMI = %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;

    
    printf("Enter loan amount: ");
    scanf("%f", &principal);

    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &rate);

    printf("Enter loan duration in months: ");
    scanf("%d", &months);

    
    calculateEMI(principal, rate, months);

    return 0;
}
```


## OUTPUT
![Screenshot 2025-05-24 192128](https://github.com/user-attachments/assets/3f42514a-d247-4310-bbc2-3caf4bc0c40a)

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
    int n = 6;
    int a = 0, b = 1, next, i;

    printf("Fibonacci series for %d terms:\n", n);

    for(i = 1; i <= n; i++) {
        printf("%d ", a);
        next = a + b;
        a = b;
        b = next;
    }

    return 0;
}
```
## OUTPUT
![Screenshot 2025-05-24 192303](https://github.com/user-attachments/assets/1400e0de-d6c4-4d00-8d74-80c4296fa236)

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
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n]; 

   
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    
    printf("Last element = %d\n", arr[n - 1]);

    return 0;
}
```
## OUTPUT

![Screenshot 2025-05-24 192450](https://github.com/user-attachments/assets/9e892a0a-3368-42c6-888c-25f5a9e3d809)

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
    int n, i, count = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    
    for (i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }

    printf("Total number of positive elements = %d\n", count);

    return 0;
}
```

## OUTPUT

![Screenshot 2025-05-24 192614](https://github.com/user-attachments/assets/46c933bc-b3ff-48d3-b73f-74f328dacd2d)

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
#include <stdio.h>

int main() {
    int n, i;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0) {
            arr[i] = -1;
        }
    }
    printf("Array after replacing even elements with 'E':\n");
    for(i = 0; i < n; i++) {
        if(arr[i] == -1) {
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
 
![Screenshot 2025-05-24 192812](https://github.com/user-attachments/assets/a5440c2c-9ec3-4e5c-93c6-b867271087c3)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



