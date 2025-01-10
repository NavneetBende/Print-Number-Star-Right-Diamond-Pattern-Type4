#include<stdio.h>
int main()
{
int i,j,r;                                      //declaring integer variables i,j for loops and r for number of rows
printf("Enter the number of rows(odd) :\n");    //Asking user for input
scanf("%d",&r);                                 //taking number of rows and saving it in variable r
for(i=0;i<r;i++)                                 // loop for number of rows
  {
    if(i<=(r/2))                                 //if condition to print the top half
      {
        for(j=0;j<=i;j++)                        // loop for digits per each row
          {
            if(j!=0)
              {
                printf("*%d",i+2);               //printing digits and stars
              }
            else
              {
                printf("%d",i+2);                 //printing digits
              }
          }
      }
    else                                          //else condition to print the bottom half
      {
        for(j=i;j<r;j++)                           //loop for printing
          {
            if(j!=i)
              {
                printf("*%d",r-i+1);                //printing stars and digit
              }
            else
              {
                printf("%d",r-i+1);                  //printing digit
              }
          }
      }

    printf("\n");                                     // printing newline after each row
  }
}
