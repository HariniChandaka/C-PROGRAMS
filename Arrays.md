## 1.Write a program in C to store elements in an arrays and print them.
```c
#include<stdio.h>
int main()
{
        int arr[100],n,i;
        printf("Enter the number of elements in the array: \n");
        scanf("%d",&n);
        printf("Enter %d elements : \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        printf("The elements in the array are: \n");
        for(i=0;i<n;i++)
        {
                printf("%d",arr[i]);

        }
        return 0;
}
```
## 2.Write a program in C to read n number of values in an array and display them in reverse order.
```c
#include<stdio.h>
int main()
{
        int arr[100],n,i;
        printf("Enter number of elements in an array: \n");
        scanf("%d",&n);
        printf("Enter %d elements : \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d", &arr[i]);
        }
        printf("the elements in the  reverse order: \n");
        for(i=n-1;i>=0;i--)
        {
                printf("%d",arr[i]);

        }
        return 0;
}

```
## 3.Write a program in C to find the sum of all elements of the  array.
```c
#include<stdio.h>
int main()
{
        int arr[100],i,n,sum=0;
        printf("Enter the number of elements in an array:");
        scanf("%d",&n);
        printf("Enter %d elements:\n",n);
        for(i=0;i<n;i++)
        {
         scanf("%d",&arr[i]);
        }
        for(i=0;i<n;i++)
        {
                sum=sum+arr[i];
        }
        printf("Sum of elements in the array are: %d\n ",sum);
        return 0;
}
```
## 4.Write a program in C to copy the elements of one array into another array.
```c
#include<stdio.h>
int main()
{
        int arr1[100],arr2[200],i,n;
        printf("Enter the number of elements in an array: \n");
        scanf("%d",&n);
        printf("Enter %d elements: \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr1[i]);
        }
        for(i=0;i<n;i++)
        {
                arr2[i]=arr1[i];
        }
        printf("The elements copied into the second array are: \n");
        for(i=0;i<n;i++)
        {
                printf("%d",arr2[i]);
        }
        return 0;
}
```
## 5.Write a program in C to count the total number of duplicate elements in an array.
```c
#include<stdio.h>
int main()
{
        int arr[100],i,j,n,count=0;
        printf("Enter the number of elements in an array: ");
        scanf("%d",&n);
        printf("Enter %d elements: \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        printf("Duplicate elements are : ");
        for(i=0;i<n;i++)
        {
                for(j=i+1;j<n;j++)
                {
                        if(arr[i]==arr[j])
                        {
                                count++;
                                printf("%d",arr[i]);
                                break;
                        }
                }
         }
        printf("\n Total number of duplicate elements:%d\n",count);
        return 0;
}

```
## 6. Write a program in C to print all unique elements in an array.  
```c
#include<stdio.h>
int main()
{
        int arr[100],i,j,n,count=0;
        printf("Enter number of elements in an array: \n");
        scanf("%d",&n);
        printf("Enter %d elements: \n ",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        printf("Unique elements are: ");
        for(i=0;i<n;i++)
        {
                count=0;
                for(j=0;j<n;j++)
                {
                        if(arr[i]==arr[j])
                        {
                          count++;
                         }
                }
                        if(count==1)
                        {
                         printf("%d",arr[i]);
                         }
                         }
        return 0;

}
```
## 7.Write a program in C to merge two arrays of the same size sorted in descending order.
```c
#include<stdio.h>
int main()
{
  
       int i,j,n,temp;
        printf("Enter the size of the array: \n" );
        scanf("%d",&n);
        printf("Enter the elements of First array: ");
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr1[i]);
        }
        printf("Enter the elements of the second array: ");
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr2[i]);
        }
        for(i=0;i<n;i++)
        {
                merged[i]=arr1[i];
        }
        for(j=0;j<n;j++,i++)
        {
                merged[i]=arr2[j];
        }
        for(i=0;i<2*n-1;i++)
        {
                for(j=i+1;j<2*n;j++)
                {
                        if(merged[i]<merged[j])
                        {
                                temp=merged[i];
                                merged[i]=merged[j];
                                merged[j]=temp;
                        }

                }
        }
        printf("merged array in descending order: \n");
        for(i=0;i<2*n;i++)
        {
                printf("%d",merged[i]);
        }
         printf("\n");
        return 0;
}

```
## 8. Write a program in C to count the frequency of each element of an array.
```c
#include<stdio.h>
int main()
{
       int arr[100],freq[100];
        int n,i,j,visited=-1;
        printf("Enter the number of elements: \n");
        scanf("%d",&n);
        printf("Enter %d elements: \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
                freq[i]=0;
        }
        for(i=0;i<n;i++)
        {
                if(freq[i]==visited)
                        continue;
                 int count=1;
                 for(j=i+1;j<n;j++)
                 {
                         if(arr[i]==arr[j])
                         {
                                 count++;
                          freq[j]=visited;
                        }
                 }
                freq[i]=count;
        }
 printf("\n Frequency elements are : \n");
 for(i=0;i<n;i++)
{
        if(freq[i]!=visited){
        printf("%d occurs %d times \n",arr[i],freq[i]);
        }
}
return 0;
}
```
## 9.Write a program in C to find the maximum and minimum elements in an array .
```c
#include<stdio.h>
int main()
{
         int arr[100],n,i,min,max;
         printf("Enter the number of elements in an array: ");
         scanf("%d",&n);
         printf("Enter %d Elements: \n",n);
         for(i=0;i<n;i++)
         {
                 scanf("%d",&arr[i]);
         }
         max=min=arr[0];
         for(i=0;i<n;i++)
         {
                 if(arr[i]>max){
                         max=arr[i];
                    }
                 if(arr[i]<min){
                         min=arr[i];
                 }
         }
         printf("Maximum elements are : %d\n",max);
         printf("Minimum elements are: %d\n",min);
          return 0;
}
```
## 10.Write a program in C to separate odd and even integers into seperate array.
```c
#include<stdio.h>
int main()
{
        int arr[100],n,i,odd[100],even[100],ecount=0,ocount=0;
        printf("Enter the number of  elements in an array: ");
        scanf("%d",&n);
        printf("Enter %d elements: \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        for(i=0;i<n;i++)
        {
                if(arr[i]%2==0)
                {
                        even[ecount]=arr[i];
                        ecount++;
                }
                else
                {
                        odd[ocount]=arr[i];
                        ocount++;
                }
        }
        printf("\n Even numbers are: \n");
        for(i=0;i<ecount;i++)
        {
                printf("%d ",even[i]);
        }
        printf("\n Odd numbers are :\n");
        for(i=0;i<ocount;i++)
        {
                printf("%d ",odd[i]);
        }
       return 0;
      }
```
## 11.Write a program in C to sort elements of an array in Ascending order.
```c

#include<stdio.h>
int main()
{
        int arr[100],n,i,j,temp;
        printf("Enter the number of elements: \n");
        scanf("%d",&n);
        printf("Enter %d elements: \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        for(i=0;i<n-1;i++)
        {
                for(j=i+1;j<n;j++)
                {
                        if(arr[i]>arr[j]){
                        temp=arr[i];
                        arr[i]=arr[j];
                        arr[j]=temp;
                   }
                }
        }
      printf("\n Array in Ascending order: \n");
      for(i=0;i<n;i++)
      {
              printf("%d ",arr[i]);

      }
        printf("\n");

      return 0;

}
```
## 12. Write a program in C to sort elements of the array in descending order.
```c
#include<stdio.h>
int main()
{
        int arr[100],i,j,n,temp;
        printf("Enter the number of elements in an array: \n");
        scanf("%d",&n);
        printf("Enter %d elements: \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        for(i=0;i<n-1;i++)
        {
                for(j=i+1;j<n;j++)
                {
                        if(arr[i]<arr[j])
                        {
                                temp=arr[i];
                                arr[i]=arr[j];
                                arr[j]=temp;
                        }
                }

         }
                printf("\n Descending order: \n");
                for(i=0;i<n;i++)
                {
                        printf("%d ",arr[i]);
                }
                printf("\n");
                return 0;
}
```
## 13.Write a program in C to delete an element at a desired position from an array.
```c
#include<stdio.h>
int main()
{
        int arr[100],i,n,pos;
        printf("Enter the number of elements in an array: \n");
        scanf("%d",&n);
        printf("Enter %d elements : \n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        printf("Enter deletion position(0-based index): ");
        scanf("%d",&pos);
                if(pos<0||pos>=n)
        {
                printf("Invalid position");
        }
                else
                {
                      for(i=pos;i<n-1;i++)
                      {
                              arr[i]=arr[i+1];
                      }
                      n--;

               printf("Array after deletion: \n");
               for(i=0;i<n;i++)
               {
                       printf("%d ",arr[i]);
                   }
               printf("\n");
              }
        return 0;
}
```
## 14.Write a program in C to find the secong largest element in an array.
```c
#include<stdio.h>
#include<limits.h>
int main()
{
        int arr[100],i,n,first,second;
        printf("Enter the number of elements in array: \n");
        scanf("%d",&n);
        if(n<2)
        {
        printf("Array must contain atleast 2 elements: \n");
        return 0;}
        printf("Enter %d elements:\n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        first = second =INT_MIN;
        for(i=0;i<n;i++){
        if(arr[i]>first)
        {
                second=first;
                first=arr[i];
        }
        else if(arr[i]>second && arr[i]<first)
                {
                        second=arr[i];
                }
        }
        if(second==INT_MIN)
        {
                printf("No second largesr element(may be all elements are equal)");
        }
        else{
                printf("The second largest element is :%d\n",second);
             }
        return 0;
}
```
## 15.Write a program in C to find the second smallest element in an array.
```c
#include<stdio.h>
#include<limits.h>
int main()
{
        int arr[100],i,n,first,second;
        printf("Enter the number of elements in an array:\n");
        scanf("%d",&n);
        if(n<2)
        {
                printf("Array must contain atleast 2 elements:");
                return 0;
        }
        printf("Enter %d elements :\n",n);
        for(i=0;i<n;i++)
        {
                scanf("%d",&arr[i]);
        }
        first = second = INT_MAX;
        for(i=0;i<n;i++)
        {
                if(arr[i]<first)
                {
                        second=first;
                        first=arr[i];
                }
                else if(arr[i]>first && arr[i]<second)
                {
                        second=arr[i];
                }
        }
        if(second==INT_MAX)
        {
                printf("No second smallest element(may be all are equal) ");
        }
        else{
                printf("second smallest element is :%d\n",second);
        }

        return 0;
}
```
## 16.Write a program in C for a 2D array of size 3*3 and print the matrix.
```c
#include<stdio.h>
int main()
{
        int matrix[3][3];
        int i,j;
        printf("Enter elements of 3*3 matrix:");
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        printf("Enter elements [%d][%d]:",i,j);
                        scanf("%d",&matrix[i][j]);
                }
        }
        printf("\n 3*3 matrix is: \n");
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        printf("%d",matrix[i][j]);

                }
        printf("\n");

        }
        return 0;
}

```
## 17.Write a program in C for adding two matrices of the same size.
```c
#include<stdio.h>
int main()
{
        int A[3][3],B[3][3],C[3][3];
        int i,j;
        printf("Enter elements of 3*3 matrix A:\n");
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        printf("A[%d][%d]: ",i,j);
                        scanf("%d",&A[i][j]);
                }
        }
        printf("Enter elements of 3*3 matrix B:\n");
        for(i=0;i<3;i++)
          {
                  for(j=0;j<3;j++)
                  {
                          printf("B[%d][%d]: ",i,j);
                          scanf("%d",&B[i][j]);
                  }
          }
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        C[i][j]=A[i][j]+B[i][j];
                }
        }
        printf("\n Resultant matrix after addition (C=A+B) : \n");
        for(i=0;i<3;i++){
                for(j=0;j<3;j++)
                {
                        printf("%d ",C[i][j]);
                }
                printf("\n");
        }
        return 0;
}

```
## 18.Write a program in C for the subtraction of two matrices.
```c
#include<stdio.h>
int main()
{
        int A[3][3],B[3][3],C[3][3];
        int i,j;
        printf("Enter elements of 3*3 matrix: \n");
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        printf("Enter elements A[%d][%d]: ",i,j);
                        scanf("%d",&A[i][j]);
                }
        }
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        printf("Enter elements B[%d][%d]: ",i,j);
                        scanf("%d",&B[i][j]);
                }
        }
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        C[i][j]=A[i][j]-B[i][j];
                }
        }
        printf("\n Resultant subtraction matrix is (C=A-B): \n");
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        printf("%d ",C[i][j]);
                }
                 printf("\n");
        }
        return 0;
}
```
## 19.Write a program in C for the multiplication of two matrices.
```c
include<stdio.h>
int main()
{

        int i,j,k,n;
        printf("Enter the size of square matrix: \n");
        scanf("%d",&n);
       int A[n][n],B[n][n],C[n][n];
        printf("Enter %d elements of A: \n",n);
        for(i=0;i<n;i++)
        {
          for(j=0;j<n;j++)
          {
                  scanf("%d",&A[i][j]);
           }
        }
        printf("Enter %d elements of B: \n",n);
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&B[i][j]);
                }
        }
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        C[i][j]=0;
                }
        }
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        for(k=0;k<n;k++)
                        {
                          C[i][j]+=A[i][k]*B[k][j];
                                }
                }
        }
        printf("The Resultant  matrix(A*B) is :\n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++){
                        printf("%d",C[i][j]);
                                        }
                                        printf("\n");
                                        }
                                        return 0;
}
```
## 20. Write a program in C for transpose of a given matrix.
```c
#include<stdio.h>
int main()
{
        int n,m,i,j;
        printf("Enter rows and columns of the matrix: ");
        scanf("%d%d",&m,&n);
        int matrix[m][n],transpose[n][m];
        printf("Enter the elements of an matrix: ");
        for(i=0;i<m;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&matrix[i][j]);
                }
        }
        for(i=0;i<m;i++)
        {
                for(j=0;j<n;j++)
                {
                        transpose[j][i]=matrix[i][j];
                }
        }
        printf("\n Original matrix \n");
        for(i=0;i<m;i++)
        {
                for(j=0;j<n;j++)
                {
                        printf("%d ",matrix[i][j]);
                }
                printf("\n");
        }
        printf("\n Transpose matrix \n");
                for(i=0;i<n;i++)
                {
                        for(j=0;j<m;j++)
                        {
                                printf("%d ",transpose[i][j]);
                        }
                        printf("\n");
                }
        }
```
## 21.Write a program in C to find the sum of the right diagonals of a matrix.
```c
#include<stdio.h>
int main()
{
        int n,i,j;
        printf("Enter the size of the square matrix: ");
        scanf("%d",&n);
        int matrix[n][n],sum=0;
        printf("Enter elements of the matrix:");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&matrix[i][j]);
                }
        }
        for(i=0;i<n;i++)
        {
                sum+=matrix[i][n-i-1];
        }
        printf("\n matrix: \n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        printf("%d ",matrix[i][j]);
                }
                printf("\n");
        }
        printf("\n sum of right diagonal=%d\n",sum);
        return 0;
}
```
## 22.Write a program in C to find the sum of the left diagonals of a matrix.
```c
#include<stdio.h>
int main()
{
        int i,j,n;
        printf("Enter the size of the square matrix:");
        scanf("%d",&n);
        int matrix[n][n], leftsum=0;
        printf("Enter the elements of an matrix: \n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&matrix[i][j]);

                }

        }
        for(i=0;i<n;i++)
        {
                leftsum+=matrix[i][i];
        }
        printf("\n matrix \n ");
                for(i=0;i<n;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                printf("%d",matrix[i][j]);

                        }
                        printf("\n");
                }
                printf("\n sum of left diagonal is: %d\n",leftsum);
                return 0;
}
```
## 23.Write a program in C to find the sum of rows and columns of a matrix.
```c
#include<stdio.h>
int main()
{
        int m,n,i,j;
        printf("Enter number of rows and columns: ");
        scanf("%d%d",&m,&n);
        int matrix[m][n];
        printf("Enter elements of a matrix: \n");
        for(i=0;i<m;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&matrix[i][j]);
                }
        }
        printf("\n matrix\n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                printf("%d",matrix[i][j]);
                        }
                        printf("\n");
                }
       printf("\n row sum\n");
       for(i=0;i<m;i++)
       {
               int rowsum=0;
               for(j=0;j<n;j++)
               {
                       rowsum+=matrix[i][j];
                }
         printf("sum of row %d :%d\n", i+1,rowsum);
       }
       printf("\n column sum \n");
       for(j=0;j<n;j++)
       {
               int columnsum=0;
               for(i=0;i<n;i++)
               {
                       columnsum+=matrix[i][j];
                }
               printf("sum of column %d :%d\n",j+1,columnsum);
        }
                                                                                                                                                                      1,1           Top
return 0;
     }
```
## 24.Write a program in C to print or display the lower triangular of a given matrix.
```c
#include<stdio.h>
int main()
{
        int i,j,n;
        printf("Enter the size of an array: ");
        scanf("%d",&n);
        int matrix[n][n];
        printf("Enter  elements of an array: \n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&matrix[i][j]);
                }
        }
        printf("\n matrix \n");
        for(i=0;i<n;i++)
        {
        for(j=0;j<n;j++)
         {
                 printf("%d",matrix[i][j]);
                }
        printf("\n");
        }
        printf("\n lower matrix\n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        if(j<=i)
                        {
                                printf("%d",matrix[i][j]);
                        }
                        else{
                                printf("0");
                        }
                  }
                printf("\n");
        }
        return 0;
}
```
## 25.Write a program in C to print or display upper triangular matrix.
```c
#include<stdio.h>
int main()
{
        int i,j,n;
        printf("Enter the size of the matrix:");
        scanf("%d",&n);
        int matrix[n][n];
        printf("Enter elements of the matrix:\n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        scanf("%d",&matrix[i][j]);
                }
        }
        printf("\n original  matrix\n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        printf("%d",matrix[i][j]);
                }
                printf("\n");
        }
        printf("\n upper traingle \n");
        for(i=0;i<n;i++)
        {
                for(j=0;j<n;j++)
                {
                        if(j>=i){
                                printf("%d",matrix[i][j]);
                        }
                        else{
                                printf("0");
                        }
                }

                        printf("\n");
            }
        return 0;
}
```
## 26.Write a program in C to calculate the determinant of a 3*3 matrix
```c
#include<stdio.h>
int main()
{
        int matrix[3][3];
        int Determinant;
        int i,j;
        printf("Enter the elements of 3*3 matrix: \n");
        for(i=0;i<3;i++)
        {
                for(j=0;j<3;j++)
                {
                        scanf("%d",&matrix[i][j]);
                }
        }
       Determinant= matrix[0][0]*(matrix[1][1]*matrix[2][2]-matrix[1][2]*matrix[2][1])-
                    matrix[0][1]*(matrix[1][0]*matrix[2][2]-matrix[1][2]*matrix[2][0])+
                    matrix[0][2]*(matrix[1][0]*matrix[2][1]-matrix[1][1]*matrix[2][0]);
       printf("Determinant of a matrix :%d\n",Determinant);
       return 0;

}
```
## 27.Write a program in C to accept two matrices and check whether they are equal.
```c

#include<stdio.h>
int main()
{
  int i,j;
  int rows,cols,flag=1;
  printf("Enter no. of rows: ");
  scanf("%d",&rows);
  printf("Enter no. of columns: ");
  scanf("%d",&cols);
  int A[rows][cols],B[rows][cols];
  printf("Enter elements of first matrix A:\n");
  for(i=0;i<rows;i++)
  {
          for(j=0;j<cols;j++)
          {
                  scanf("%d",&A[i][j]);

        }
  }
  printf("Enter elements of second matrix B:\n");
  for(i=0;i<rows;i++)
  {
          for(j=0;j<cols;j++)
          {
                  scanf("%d",&B[i][j]);
                 }
  }
  for(i=0;i<rows;i++)
  {
          for(j=0;j<cols;j++)
          {
                  if(A[i][j]!=B[i][j])
                  {

                          flag=0;
                          break;}

                  }
          if(flag==0);
          break;
  }
  if(flag==1)
  {
          printf(" matrices are equal");}
 else{
                  printf("matrices are not equal");
          }
          return 0;
 }
```















