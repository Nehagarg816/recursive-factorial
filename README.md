# recursive-factorial
This is a program for finding factorial using recursion in functions as an alternative way instead of loop.
#include<stdio.h>
#include<conio.h>
int factorial(int a);

void main()
{
	int a,s;
	printf("Enter one number a:");
	scanf("%d",&a);
	s=factorial(a);
	printf("Factorial of a is %d",s);
}
int factorial(int x)
{
	int fact;
	if(x==1 || x==0)
	{
		return 1;
	}
	else
	{
		fact=x*factorial(x-1);
	}
	return(fact);
}
