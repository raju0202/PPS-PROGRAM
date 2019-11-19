PROGRAMMING FOR PROBLEM SOLVING
NAME-AMAN KUMAR GANDHI
BRANCH-IT
SECTION-A1
ROLL NO.-1921008
LOGO

1.Programs to display a welcome message using puts
#include<stdio.h>
int main()
{
puts("\nHELLO TO BUDDING ENGINEERS\n");
return 0;
}
Output of program

HELLO TO BUDDING ENGINEERS
2. programs to display address using puts
#include<stdio.h>
int main()
{
puts("AMAN KUMAR GANDHI \nITA1 1921008 \nGNDEC LUDHIANA,PUNJAB\n");
return 0;}
output of programs

AMAN KUMAR GANDHI
ITA1 1921008
GNDEC LUDHIANA,PUNJAB
3.programs to find the sum of two number .
#include <stdio.h>
int main()
{
    int firstNumber, secondNumber, sumOfTwoNumbers;
    
    printf("enter the two integer ");
    scanf("%d %d", &firstNumber, &secondNumber);
    sumOfTwoNumbers = firstNumber + secondNumber;      
    printf("%d + %d = %d", firstNumber, secondNumber, sumOfTwoNumbers);
    return 0;
}
Output of programs

Enter two integers: 12
11
12 + 11 = 23
4.prorams to convert Centigrate to fahrenheit .
#include<stdio.h>
int main()
{
	
	float cen, fah;
	printf("Enter temperature in Celsius : ");
	scanf("%f",&cen);
	fah=(1.8 * cen) + 32;
	printf("\nTemperature in Fahrenheit = %f",fah);
	return 0;
}
output of programs

Enter the temerature in Celsious : 37
Temperatur in fahrenheit : 98.599998
5.programs to find the area and perimeter of circle .
#include<stdio.h>
int  main()
{

	float r, area, circum;
	printf("Enter the radius of the circle :");
	scanf("%f",&r);
	area=3.14*r*r;
	circum=2*3.14*r;
	printf("Area of the circle = %f\nCircumference of the circle = %f\n",area,circum);
	return 0;
}
output of programs :

Enetr the radius of the circle :5
Area of the circle =78.500000
Circumference of the circle = 31.400000
6. program to swap the two number without using third variable .
#include<stdio.h>  
 int main()    
{    
int a=10, b=20;      
printf("Before swap a=%d b=%d",a,b);      
a=a+b;//a=30 (10+20)    
b=a-b;//b=10 (30-20)    
a=a-b;//a=20 (30-10)    
printf("\nAfter swap a=%d b=%d",a,b);    
return 0;  
}   
Output:

Before swap a=10 b=20
After swap a=20 b=10
7. programs to check whether even or odd number .
#include<stdio.h>
int main()
{
    int num;
    printf("Enter any number: ");
    scanf("%d", &num);
    if(num%2 == 0)
        printf("\nIt's an even number.");
    else
        printf("\nIt's an odd number.");
	
    return 0;
}
Output of programs

Enter any number:4
It's an even number.
8.program to find the factorial of the number .
#include<stdio.h>
int main()
{
    int num, i, fact=1;
    printf("Enter any number: ");
    scanf("%d", &num);
    for(i=num; i>0; i--)
        fact = fact*i;
    printf("\nFactorial of %d = %d", num, fact);
    
    return 0;
}
Output the programs

Enter any number:5
factorial of 5 = 120
9. programs to fizz buzz
#include <stdio.h>

int main(void)
{
    int i;
    for(i=1; i<=100; i++)
    {
        if(((i%3)||(i%5))== 0)
            printf("number= %d FizzBuzz\n", i);
        else if((i%3)==0)
            printf("number= %d Fizz\n", i);
        else if((i%5)==0)
            printf("number= %d Buzz\n", i);
        else
            printf("number= %d\n",i);

    }

    return 0;
}
Output the programs

1
2
fizz
4
buzz
..........
10.program to print week of days using switch case
#include <stdio.h>

int main()
{
    int week;
   
    printf("Enter week number(1-7): ");
    scanf("%d", &week);
    
    switch(week)
    {
        case 1: 
            printf("Monday");
            break;
        case 2: 
            printf("Tuesday");
            break;
        case 3: 
            printf("Wednesday");
            break;
        case 4: 
            printf("Thursday");
            break;
        case 5: 
            printf("Friday");
            break;
        case 6: 
            printf("Saturday");
            break;
        case 7: 
            printf("Sunday");
            break;
        default: 
            printf("Invalid input! Please enter week number between 1-7.");
    }

    return 0;
}
Output of programsg

Input week number(1-7): 2
Tuesday
11. program to make a calculator using switch case
#include<stdio.h>
int main() {
    char operator;
    double firstNumber,secondNumber;
    printf("Enter an operator (+, -, *,): ");
    scanf("%c", &operator);
    printf("Enter two operands: ");
    scanf("%lf %lf",&firstNumber, &secondNumber);
    switch(operator)
    {
        case '+':
            printf("%.1lf + %.1lf = %.1lf",firstNumber, secondNumber, firstNumber + secondNumber);
            break;
        case '-':
            printf("%.1lf - %.1lf = %.1lf",firstNumber, secondNumber, firstNumber - secondNumber);
            break;
        case '*':
            printf("%.1lf * %.1lf = %.1lf",firstNumber, secondNumber, firstNumber * secondNumber);
            break;
        case '/':
            printf("%.1lf / %.1lf = %.1lf",firstNumber, secondNumber, firstNumber / secondNumber);
            break;
        
        default:
            printf("Error! operator is not correct");
    }
    
    return 0;
}
Output

Enter an operator (+, -, *,): *
Enter two operands: 1.5
4.5
1.5 * 4.5 = 6.8
12. programs to check leap of year
#include <stdio.h>
int main()
{
    int year;
    printf("Enter a year: ");
    scanf("%d",&year);
    if(year%4 == 0)
    {
        if( year%100 == 0)
        {
            
            if ( year%400 == 0)
                printf("%d is a leap year.", year);
            else
                printf("%d is not a leap year.", year);
        }
        else
            printf("%d is a leap year.", year );
    }
    else
        printf("%d is not a leap year.", year);
    
    return 0;
}
Output 1

Enter a year: 1900
1900 is not a leap year.
13. program to check prime number or not
#include <stdio.h>
int main()
{
    int n, i, flag = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    for(i = 2; i <= n/2; ++i)
    {
       
        if(n%i == 0)
        {
            flag = 1;
            break;
        }
    }
    if (n == 1) 
    {
      printf("1 is neither a prime nor a composite number.");
    }
    else 
    {
        if (flag == 0)
          printf("%d is a prime number.", n);
        else
          printf("%d is not a prime number.", n);
    }
    
    return 0;
}
Output

Enter a positive integer: 29
29 is a prime number.
14.program to fibonacci series
#include <stdio.h>
int main()
{
    int i, n, t1 = 0, t2 = 1, nextTerm;
    printf("Enter the number of terms: ");
    scanf("%d", &n);
    printf("Fibonacci Series: ");
    for (i = 1; i <= n; ++i)
    {
        printf("%d, ", t1);
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    return 0;
}
Output

Enter the number of terms: 10
Fibonacci Series: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 
15. program to print simple matrix in array
#include <stdio.h>
int main() {
  int values[5];
  printf("Enter 5 integers: ");
  
  for(int i = 0; i < 5; ++i) {
     scanf("%d", &values[i]);
  }
  printf("Displaying integer");
  for(int i = 0; i < 5; ++i) {
     printf("%d\n", values[i]);
  }
  return 0;
}
Output

Enter 5 integers: 1
-3
34
0
3
Displaying integers: 1
-3
34
0
3
16. program to find square of number using function
#include<stdio.h>

int square(int); 

int main()
{
     int number, answer;
    
     printf("Enter your number:");
     scanf("%d", &number);
    
     answer = square(number);  
    
     printf("Square of %d is %d.", number, answer);
}

int square(int n)
{
     
     return(n*n); 
}
Output of the Program:

Enter your number:5
Square of 5 is 25.
17.program to swap a number by call by value
#include <stdio.h>
 
 
void swap(int, int);
 
int main()
{
   int x, y;
 
   printf("Enter the value of x and y\n");
   scanf("%d%d",&x,&y);
 
   printf("Before Swapping\nx = %d\ny = %d\n", x, y);
 
   swap(x, y); 
 
   printf("After Swapping\nx = %d\ny = %d\n", x, y);
 
   return 0;
}
 
void swap(int a, int b)
{
   int temp;
 
   temp = b;
   b = a;
   a = temp;
    printf("Values of a and b is %d  %d\n",a,b);
}
Output:

Enter the value of x and y
Before Swapping
x = 10
y = 5
Values of a and b is 5 10
After Swapping
x = 10
y = 5
18.program to swap two number by call by reference
#include <stdio.h>
 
int main()
{
  int x, y, t;
 
  printf("Enter two integers\n");
  scanf("%d%d", &x, &y);
 
  printf("Before Swapping\nFirst integer = %d\nSecond integer = %d\n", x, y);
 
  t = x;
  x = y;
  y = t;
 
  printf("After Swapping\nFirst integer = %d\nSecond integer = %d\n", x, y);
 
  return 0;
}
The output of the program:

Enter two integers
23
45
Before Swapping
First integer = 23
Second integer = 45
After Swapping
First integer = 45
Second integer = 23
19.program to find factorial of number using recursion
#include<stdio.h>
int find_factorial(int);
int main()
{
   int num, fact;
   
   printf("\nEnter any integer number:");
   scanf("%d",&num);
 
   
   fact =find_factorial(num);
 
   
   printf("\nfactorial of %d is: %d",num, fact);
   return 0;
}
int find_factorial(int n)
{
   
   if(n==0)
      return(1);
 
   
   return(n*find_factorial(n-1));
}
Output:

Enter any integer number: 4

factorial of 4 is: 24
