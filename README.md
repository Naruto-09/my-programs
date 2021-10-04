# my-programs
Only for coding purpose
#include<stdio.h>
void operation(int temp[3][3])
{
      int i,j,flag=0;
      for(i=0;i<=2;i++)
      {
            for(j=0;j<=2;j++)
            {
                  if(i<j   &&  temp[i][j])
                  {
                        flag=1;
                        break;
                 }
          }
      }   if(flag==1)
           {
                 printf("\n not lower triangular matrix");
           }
           else
           {
                 printf("\n lower triangular matrix");
           }
           
}
void main()
{
      int a[3] [3];
      int i,j;
      printf("Enter the elements of an array");
      for(i=0;i<=2;i++)
      {
            for(j=0;j<=2;j++)
            {
                  scanf("%d",&a[i][j]);
            }
      }
      printf("matrix elements are \n");
      for(i=0;i<=2;i++)  
      {
            for(j=0;j<=2;j++)
            {
                  printf("%d\t",a[i][j]);
                  
            }
            printf("\n");
        }
        printf("\n Your matrix result is in \n");
        operation(a);
        
}
