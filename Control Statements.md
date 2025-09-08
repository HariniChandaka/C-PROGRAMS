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
## 14.Write a c program to find maximum between two numbers using switch case?
```c
#include <stdio.h>
int main()
{
    int a,b,choice;
    printf("Enter two numbers:");
    scanf("%d%d",&a,&b);
    choice=(a>b) ? 1 :((b<a) ? 2 : 0);
    switch(choice)
    {
        case 1:printf("maximum number is: %d\n",a);
               break;
        case 2:printf("maximum number is: %d\n",b);
               break;
        case 3:printf("both numbers are equal \n");
               break;
        default:printf("invalid input");
    }
}
```
## 15.Write a c program to print even numbers between 1 to 20 using a for loop?
```c
int main()
{
    int i;
    printf("Even numbers between 1 to 20 are: \n");
    for(i=1;i<=20;i++)
    {
        if(i%2==0)
        {
            printf("%d \n", i);
        }
    }
    return 0;
}
```
## 16.Write a c program to calculate the sum of numbers from 1 to 100 using a while loop?
```c
#include<stdio.h>
int main()
{
    int i=1;
    int sum=0;
    while(i <= 100)
    {
        sum += i;
        i++;
    }
    printf("The sum of numbers from 1 to 100 is: %d\n",sum);
    return 0;
}
```
## 17.Write a c program to find the factorial of a given number using a for loop?
```c
#include <stdio.h>
int main()
{
    int num,i;
    unsigned long long factorial=1;
    printf("Enter a number:");
    scanf("%d",&num);
    if(num<0)
    {
        printf("factorial is not defined for negative values.\n");
    }
    else
    {
        for(i=1;i<=num;i++)
        {
            factorial=factorial*i;
        }
            printf("factorial of %d=%llu\n",num,factorial);
    }
    return 0;
}
```
## 18.Write a c program to check whether a given number is prime or not using a while loop?
```c
#include<stdio.h>
int main()
{
    int num,i=2,isprime=1;
    printf("Enter a number:");
    scanf("%d",&num);
    if(num<=1)
    {
        isprime=0;
    }
    else
    {
        while(i<=num/2);
        {
          if(num%i==0)
         {
           isprime=0;
         }
          i++;
        }
    }
    if(isprime)
    printf("%d is a prime number: \n",num);
    else
    printf("%d is not a prime number: \n",num);
    return 0;
}
```
## 19..Write a c program to find the sum of digits of a number using a while loop?
```c
#include <stdio.h>
int main()
{
    int n,sum=0,digit;
    printf("Enter the number: ");
    scanf("%d",&n);
    while(n>0)
    {
      digit=n%10;
      sum=sum+digit;
      n=n/10;
      printf("sum of digits: %d\n",sum);
    }
    
}
```
## 20.. Write a c program to print fibonacci series up to n terms using a for loop?
```c
#include <stdio.h>
int main()
{
    int n,i;
    int first=0,second=1,next;
    printf("Enter the number of terms:");
    scanf("%d",&n);
    printf("fibonacci series upto %dterms : ",n);
    for(i=0;i<=;i++)
    {
        printf("%d",first);
        next=first+second;
        first=second;
        second=next;
    }
    return 0;
}
```
## 21.Write a c program to reverse a given number using a while loop
```c
#include <stdio.h>
int main()
{
    int i=0,j=0,digit;
    printf("Enter the number:");
    scanf("%d",&i);
    while (i>0)
    {
        digit=i%10;
        j=(j*10)+digit;
        i=i/10;
        printf("reverse value is: %d\n",j);
    }
    return 0;
}
```
## 22.Write a c program to find the largest element in an array using a for loop?
```c
#include <stdio.h>
int main()
{
    int arr[100],i,n,max;
    printf("Enter the number of elements in an array: ");
    scanf("%d",&n);
    
    printf("Enter %d elements: \n",n);
    for(i=0;i<n;i++)
    {
    scanf("%d",&arr[i]);
    }
     max=arr[0];
       for(i=1;i<n;i++)
       {
           if(arr[i]>max)
           {
             max=arr[i];
           }
       }
    printf("largest elements in the array is : %d\n",max);
    
    return 0;       
}
```
## 23.Write a c program to find the smallest element in an array using a while loop?
```c
#include <stdio.h>
int main()
{
    int arr[100],i,n,min;
    printf("Enter the number of elements in an array");
    scanf("%d",&n);
    printf("Enter %d elements: \n",n);
    for(i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    min=arr[0];
    for(i=1;i<n;i++)
    {
        if(arr[i]<min)
        {
            min=arr[i];
        }
    }
    printf("smallest elements in the array is : %d \n",min);
    return 0;
}
```
## 24.Write a c program to print all the elements of an array using a for loop? 
```c
#include <stdio.h>
int main()
{
    int arr[100],i,n,max;
    printf("Enter the number of elements in an array: ");
    scanf("%d",&n);
    
    printf("Enter %d elements: \n",n);
    for(i=0;i<n;i++)
    {
    scanf("%d",&arr[i]);
    }
    printf("The elements of the array are: \n");
    for(i=0;i<n;i++)
    {
    printf("%d",arr[i]);
    }
    printf("\n");
    return 0;
}
```
##  25.Write a c program to find the sum of elements in an array using a while loop?
```c
#include <stdio.h>
int main()
{
    int n,i=0,sum=0;
    printf("Enter the number of elements in an array:");
    scanf("%d",&n);
    int arr[n];
    printf("Enter %d elements: \n",n);
    while(i<n)
    {
        scanf("%d",&arr[i]);
    }
    
    i=0;
    while(i<n)
    {
        sum=sum+arr[i];
        i++;
    }
    printf("The sum of the elements in the array is: %d\n",sum);
    return 0;
}
```
## 26  
 


   







