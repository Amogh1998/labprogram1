//roots of a quadratic equation
#include<stdio.h>
##include<math.h>
int main()
{
	float a,b,c,d,rr,ir,r1,r2;
	printf("Enter the co-efficients : " );
	scanf("%f%f%f",&a,&b,&c);
	d=(b*b)-(4*a*c);           //determinant calculation
	if(d=0)
	{
		r1=r2=0;
		printf("\nThe roots are real and equal\nroot r1 is : %f\nthe root r2 is ; %f ",r1,r2);
	}
	else if(d>0)
 	{
		r1=(-b+sqrt(d))/(2*a);
		r2=(-b-sqrt(d))/(2*a);
		printf("\nThe roots are real and distinct\nThe root r1 is : %f\n The root r2 is : %f ",r1,r2);
	}
	else
	{
		rr=-b/(2*a);
		ir=sqrt(-d)/(2*a);
		printf("\nThe roots are complex\nthe root r1 is : %f + %f i\nThe root r2 is : %f + %f i ",rr,ir,rr,ir);
	}
	return 0;
}
