PRINTING PATTERN:
2

3*3

4*4*4

3*3

2

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows as input from the user and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r. The loop should be structured as for( i=0 ; i<r : i++).
Use an if condition to to print the top half of the triangle. if (i<=r/2). Then run a loop from j=0 to j<=i. The loop should be structured as for(j=0 ; j<=i ; j++)
Run a nested if statement if(j!=0)  then print star and i+2.
Else print only i+2.
Else statement for the outer if statement: run a loop from j=i to j<r. The loop should be structured as for(j=i ; j<r; j++)
Inside this loop run an if statement if(j!=i) then print star and r-i+1.
Else just print r-i+1.
Inside the main loop print a newline to move to the next line after each row is printed.
CODE IN C:
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
TAKING INPUT:DISPLAYING OUTPUT:
