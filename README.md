# sample
#include <stdio.h>

  int fact( );
  void prime_non();
  void odd_even();
  int main()
  {
     int i,n,choi;
     while(1)
     {
      printf("\n Enter 1 for factorial ");
      printf("\n Enter 2 for checking prime or non prime ");
      printf("\n Enter 3  for checking odd or even");
      printf("\n Enter 4 for Exit ");
      printf("\n Enter your choice : ");
      scanf("%d", &choi);
      switch(choi)
      {
          case 1:
             fact(n);
             break;
          case 2:
             prime_non(n);
             break;
          case 3:
             odd_even(n);
             break;
          case 4:
            exit (0);
            break;
      }
     }

      return 0;
  }
  int fact() 
  {
      int i,n ,f=1;
      printf("\nenter the no :");
      scanf("%d", &n);
      for(i=1; i<=n; i++)
      {
          
          f = i*f;
          
      }
       printf("\n factorial of %d = %d", n,f);
       return (f);
  }
  void prime_non()
  {
      int n,i, f=1;
      printf("\nenter the no :");
      scanf("%d", &n);
      if (n==1)
        f=0;
      else
      {
          for(i=2; i<n ; i++)
          {
              if(n%i==0)
              {
                f=0;
                break;
              }
          }
          
      }
      if(f==1)
            printf("\n %d is  prime no",n);
      else
            printf("\n %d is non prime no",n); 
  }
  void odd_even()
  {
      int n;
      printf("\nenter the no :");
      scanf("%d", &n);
      if(n%2==0)
         printf("\n %d is an even no", n);
      else
         printf("\n %d is an odd no", n);
      
  }
