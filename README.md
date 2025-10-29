EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
```

#include <stdio.h>
#include<math.h>
int main() {
float m=23.65;
float *p=&m;
printf("%.0f",ceil(*p)+1);
}

```
## OUTPUT:
 <img width="469" height="239" alt="image" src="https://github.com/user-attachments/assets/59240eff-2a2f-4e9f-b67d-513f7d685401" />












## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
```
#include <stdio.h>
int add(int n)
{
    
    if(n==1)
    return 1;
    return n*add(n-1);
}
int main() {
   int n=12;
   int sum=add(n);
   printf("Product of first 12 natural numbers : %d",sum);
}
```
## OUTPUT:
<img width="543" height="248" alt="image" src="https://github.com/user-attachments/assets/0809f1ee-d64f-4399-8a07-c8eb42bcf375" />
	
## RESULT:

Thus the program has been executed successfully.
 
 


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:
```

#include <stdio.h>

int main() {
   int m,n,sum1=0,sum2=0,sum3=0,i,j;
   scanf("%d%d",&m,&n);
   int a[m][n];
   for(i=0;i<m;i++)
   {
       for(j=0;j<n;j++)
       scanf("%d",&a[i][j]);
   }
    for(j=0;j<n;j++)
    {
        i=0;
        sum1+=a[i][j];
    }
     for(j=0;j<n;j++)
     {
         i=1;
         sum2+=a[i][j];
     }
      for(j=0;j<n;j++)
      {
          i=2;
          sum3+=a[i][j];
      }
      printf("Sum of 1st row : %d\nSum of 2nd row : %d\nSum of 3rd row : %d\n",sum1,sum2,sum3);
}
   
```


## OUTPUT
<img width="478" height="357" alt="image" src="https://github.com/user-attachments/assets/528f27dd-920d-4d0f-8e31-bd5dd97c641b" />


 
 

 ## RESULT
 


# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
  int n;
  scanf("%d",&n);
  char str[50];
  scanf("%s",str);
  for(int i=0;i<n;i++)
  {
      for(int s=0;s<=n-i-1;s++){
      printf("    ");
      }
          for(int j=0;j<=i;j++)
          {
          printf("%s ",str);
          }
          printf("\n");
      
  }
}
```

 ## OUTPUT
<img width="592" height="366" alt="image" src="https://github.com/user-attachments/assets/3b9d58e2-8b88-42c6-8046-52fbd6362980" />

 

## RESULT

Thus the C program to String process executed successfully
 

 
.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM
```
#include <stdio.h>

int main() {
  int n;
  scanf("%d",&n);
  int a[n];
  for(int i=0;i<n;i++)
  {
  scanf("%d",&a[i]);
  }
  int *p=a;
  for(int i=0;i<n;i++)
  {
      printf("%d ",*p);
      p++;
  }
}
```
## OUTPUT
<img width="551" height="298" alt="image" src="https://github.com/user-attachments/assets/46b67601-cbdb-4ff6-8db3-cca00f20f32d" />


## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


