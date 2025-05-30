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
void cemi(float p, float r, float n) {
    float emi;   
    r = r / (12 * 100); 
    n = n * 12;  
    emi = (p * r * pow(1 + r, n)) / (pow(1 + r, n) - 1);
    printf("Monthly EMI is= %.3f\n", emi);
}
int main() {
   float principal, rate, time;
   scanf("%f %f %f", &principal, &rate, &time);
   cemi(principal, rate, time);
   return 0;
}
```
## OUTPUT


![438184909-3d6d442b-4c67-4774-b910-ca7fb5cfc795](https://github.com/user-attachments/assets/ec6c00de-1485-45cd-ba4d-1a44f83fab24)

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
#include<stdio.h>
int main(){
    int a=0,b=1,c,i,n;
    scanf("%d",&n);
    for(i=1;i<=n;i++){
        c=a+b;
        printf("%d ",a);
        a=b;
        b=c;
    }
    return 0;    
}
```

## OUTPUT


![438187487-37d3a0de-c020-451a-8318-b01c9b8878bf](https://github.com/user-attachments/assets/027cd280-0576-466d-a5f7-a6e3664b1061)

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
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
        printf("%d ",a[n-1]);
    return 0;
}
```

## OUTPUT


![438185489-b2236124-a5c4-4718-a195-cab41c548ee4](https://github.com/user-attachments/assets/da352185-b9f9-4fa8-83e2-34f3cd8d27bb)



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
#include<stdio.h>
int main()
{
    int n,count=0;
    scanf("%d",&n);
    int arr[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<n;i++)
    {
        if(arr[i]<0)
        {
            count++;
        }
    }
    printf("count  of positive numbers  in array: %d",count);
    return 0;
}
```


## OUTPUT

![438186259-9c62d6c0-553c-4f30-9bbb-cf3e9c001236](https://github.com/user-attachments/assets/77d9ecaa-406d-4fd9-9eff-fa69d649b313)


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

int n;
printf("Enter Number of elements:");
scanf("%d", &n);
int arr[n];
printf("Enter elements:");
for (int i = 0; i < n; i++) {
    scanf("%d", &arr[i]);  
    if (arr[i] % 2 == 0) arr[i] = 'E'; 
}
for (int i = 0; i < n; i++) {
    if (arr[i] == 'E') {
        printf("E "); 
    } else {
        printf("%d ", arr[i]); 
    }
}

return 0;
}
```
## Output:
 
![438186458-d719a89b-8e69-4f48-80b6-1f03c054ba8c](https://github.com/user-attachments/assets/22434349-b547-4459-bbbe-e3c246925157)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



