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
## 4.Write a C program whether a given year is leap year or not?
```c
#include <stdio.h>
int main()
{
    int year;
    printf("Enter the year: \n");
    scanf("%d",&year);
    if(year % 4==0 && year %100!==0 && year % 400==0)
     {
        printf("%d is a leap year \n",year);
    }
    else
    {
        printf("%d is not a leap year \n",year);
    }
}
```
## 5.Write a C program to read the age of a candidate and determine whether he is eligible to cast his/her own vote?
```c
#include <stdio.h>
int main()
{
    int age;
    printf("Enter the age:");
    scanf("%d",&age);
    if(age>=18)
    {
    printf("Eligible to cast his/her vote");
    }
    else if(age<=18) 
    {
        printf("Not eligible to cast his/her vote");
    }
}
```
## 6.Write a C program to read the value of an integer m and display the value of n is 1 when m is larger than 0, 0 when m is 0 and -1 when m is less than 0.
```c
#include <stdio.h>
int main()
{
    int M;
    printf("Enter the value of M:");
    scanf("%d",&M);
    if(M>0)
    {
    printf("N=1");
    }
    else if(M==0)
    {
        printf("M==0");
    }
    else if(M<0)
    {
        printf("M<0");
    }
}
```
## 7.Write a C program to find the largest of three numbers?
```c
#include <stdio.h>
int main()
{
  int num1,num2,num3 ;
      printf("Enter the three num :");
      scanf("%d %d %d",&num1,&num2,&num3);
  if(num1>=num2 && num1>=num3)
  {
      printf("the number is: %d,\n",num1);
  }
  else if(num2>=num1 && num2>=num3)
  {
      printf("the number is: %d,\n",num2);
  }
  else
  {
  printf("the number is: %d,\n",num3);
  }  
}  
```
## 8.Write a C program to check whether a character is a vowel or consonant?
```c
#include <stdio.h>
int main()
{
    char ch;
    printf("Enter an alphabet:");
    scanf(" %c",&ch);
    if((ch >= 'A'&& ch<='Z')||(ch>='a'&& ch<='z'))
    {
        char lower= ( ch >='A'&& ch<='Z') ?ch + 32:ch;
        if(lower =='a'||lower =='e'||lower =='i'||lower =='o'||lower =='u')
        {
            printf("The character %c is vowel.\n",ch);
        }
        else
        {
            printf("The character %c is a constant.\n",ch);
        }
    }    
        else
        {
            printf("%c is not an alphabet.\n",ch);
        }
    
    return 0;
}

```
## 9.Write a c program to check whether a character is an alphabet or not?
```c
#include <stdio.h>
int main()
{
    char ch;
    printf("Enter an alphabet:");
    scanf(" %c",&ch);
    if((ch >= 'A'&& ch<='Z')||(ch>='a'&& ch<='z'))
    
        {
            printf("The character %c is an alphabet.\n",ch);
        }
        else
        {
            printf("The character %c is not an alphabet.\n",ch);
        }
       return 0;
}
```
## 10.Write a c program to find minimum or maximum between two numbers?
```c
#include <stdio.h>
int main()
{
    int num1,num2;
    printf("Enter two numbers:");
    scanf("%d %d",&num1,&num2);
    if(num1>num2)
    {
        printf("maximum number is: %d\n",num1);
        printf("minimum number is: %d\n",num2);
    }
    else if(num2>num1)
    {
        printf("maximum number is: %d\n",num2);
        printf("minimum number is: %d\n",num1);
    }
    else 
    {
        printf("Both numbers are equal: %d\n",num1,num2);
    }
}
```
## 11.Write a C program to enter week number and print day of week?
```c
#include <stdio.h>
int main()
{
    int day;
    {
        printf("Enter the day :");
        printf("with in the range 1-7");
        scanf("%d",&day);
    }
    switch(day)
    {
        case 1: printf("sunday");
        break;
        case 2: printf("monday");
        break;
        case 3: printf("tuesday");
        break;
        case 4:printf("wednesday");
        break;
        case 5: printf("thursday");
        break;
        case 6: printf("friday");
        break;
        case 7: printf("saturday");
        break;
        default: printf("invalid input");
    }
}  
```
## 12.Write a Cprogram to check whether a character is uppercase or lowercase?
```c
#include <stdio.h>
int main()
{
    char ch;
    printf("Enter the character:");
    scanf(" %c",&ch);
    if(ch >= 'A' && ch <= 'Z')
    {
        printf("The character is uppercase: %c",ch);
    }
    else if(ch >= 'a' && ch <= 'z')
    {
        printf("The character is lowercase: %c",ch);
    }
    else
    {
        printf("The character is not an alphabet %c",ch);
    }
}
```
## 13.Write a C program to find number of days in month?
```c
#include<stdio.h>
int main()
{
  int month;
  printf("Enter the month :");
  printf("with in a range of 1-12:");
  scanf("%d",&month);
  switch(month)
  {
      case 1:printf("31 days");
      break;
      case 2:printf("28 0r 29 days");
      break;
      case 3:printf("31 days");
      break;
      case 4:printf("30days");
      break;
      case 5:printf("31 days");
      break;
      case 6:printf("30days");
      break;
      case 7:printf("31 days");
      break;
      case 8:printf("31 days");
      break;
      case 9:printf("30days");
      break;
      case 10:printf("31 days");
      break;
      case 11:printf("30days");
      break;
      case 12:printf("31 days");
      break;
      default:printf("invalid input");
  }
}
```
