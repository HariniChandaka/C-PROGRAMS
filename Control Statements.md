## 1.Write a program to accept two integers and check whwther they are equal or not?
```c
#include <stdio.h>
int main()
{
    int num1,num2;
    printf("Enter the first number:");
    scanf("%d",&num1);
    printf("Enter the second number:");
    scanf("%d",&num2);
    if(num1==num2)
    {
        printf("The number is equal");
    }
    else if(num1!=num2)
    {
        printf("The number is not equal");
    }
}
```
## 2.Write a C program to check whether a given number is even or not?
```c
#include <stdio.h>
int main()
{
 int number;
 printf("Enter your number:");
 scanf("%d",&number);
 if(number%2==0)
{
    printf("The number is Even \n");
}
else if(number%2!=0)
{
    printf("The number is odd \n");
}
return 0;
}
```
## 3.Write a C program to check whether a given number is positive or negative?
```c
#include <stdio.h>
int main()
{
 int number;
 printf("Enter your number:");
 scanf("%d",&number);
 if(number>0)
{
    printf("The number is positive \n");
}
else if(number<0)
{
    printf("The number is negative \n");
}
else 
{
    printf("The number is zero \n");
}
return 0;
}
```
