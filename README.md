# Write-a-program-using-switch-case-to-display-a-menu-that-offers-5-options-read-three-numbers-calcu
#include<stdio.h>
void main()
{
         int choice,x,y,z,largest,Smallest;
        printf("The options are given below, Select as per your choice\n");
        printf(" 1-Read the numbers \n 2-Calculate total \n 3- Calculate Average \n 4- Display the Smallest \n 5- Display the largest");
          printf("\n\nYour Choice :-  ");
    scanf("%d",&choice);
   switch(choice)
    {
        case 1 : printf("Enter the numbers :- \n");
                 scanf("%d %d %d",&x,&y,&z);
                 break;
                 
        case 2 : printf("Enter the numbers :- \n");
                 scanf("%d %d %d",&x,&y,&z);
                 printf("Total = %d", x+y+z);
                 break;
                 
        case 3 : printf("Enter the numbers :- \n");
                 scanf("%d\n %d %d",&x,&y,&z);
                 printf("Average = %d", (x+y+z)/3);          
                 break;
                 
        case 4 : printf("Enter the numbers :- \n");
                 scanf("%d\n%d\n %d",&x,&y,&z);
                 if(x > y)
                  {
                      if(x > z)
                      largest = x;
                      else
                      largest = z;
                  }
                  else
                  {
                      if(y > z)
                      largest = y;
                      else
                      largest = z;
                  }
                  printf("Largest among the three numbers is %d", largest);
         
        case 5 : printf("Enter the numbers :- \n");
                 scanf("%d\n%d\n %d",&x,&y,&z);
                 if(x<y)
                  {
                      if(x<z)
                      Smallest = x;
                      else
                      Smallest = z;
                  }
                  else
                  {
                      if(y<z)
                      Smallest = y;
                      else
                      Smallest = z;
                  }
                  printf("Smallest among the three numbers is %d", Smallest);
                  break;
                  
        default : printf("Wrong input");
                   break;
               }
getch();
}

