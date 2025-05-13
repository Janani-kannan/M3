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
#include <math.h>
#include <stdio.h>
float Calculate_EMI(float p, float r, float t){
   float emi;
   r = r / (12 * 100); // one month interest
   t = t * 12; // one month period
   emi = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
   return (emi);
}
int main(){
   float principle=251000, rate=8.5, time1=5, emi;
   emi = Calculate_EMI(principle, rate, time1);
   printf("Monthly EMI is= %.3f", emi);
   return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/e92036d9-5582-44fc-bd30-d3a74a86b48b)




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
    int n = 11; 
    int first = 0, second = 1, next;

 

    for (int i = 0; i < n; i++) {
        if (i <= 1)
            next = i; 
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }

    printf("\n");
    return 0;
}
```
## OUTPUT

![image](https://github.com/user-attachments/assets/64b23d5a-dfb4-4e77-9403-2a38d83de711)





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
int main()
{
    int a,i;
    scanf("%d",&a);    
    int x[a];

    for (i=0;i<a;i++)
    {
        scanf("%d",&x[i]);
        if (i%2!=0)
            printf("%d ",x[i]);

    }
    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/516d4e5e-cc30-49d9-bf65-ce734f66f4a1)



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
    int n, i;
    int positive = 0, negative = 0;
    scanf("%d", &n);

    int a[n];
    for (i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }

    for (i = 0; i < n; i++) {
        if (a[i] > 0) {
            positive++;
        } else if (a[i] < 0) {
            negative++;
        }
    }

    printf("count  of positive numbers  in array: %d\n", positive);
    printf("count  of negative numbers  in array: %d\n", negative);

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/ed7bf320-4d7a-4222-9e8c-f6d1364c502d)


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

    printf("Array after replacing even elements with 'E':\n");
    for(i = 0; i < n; i++) {
        if(arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
```

## Output:
 
![image](https://github.com/user-attachments/assets/8af33b34-ac95-4db3-844c-1e17df8c3804)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



