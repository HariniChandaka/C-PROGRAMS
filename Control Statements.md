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
