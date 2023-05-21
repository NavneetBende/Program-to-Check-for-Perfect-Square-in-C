# Program-to-Check-for-Perfect-Square-in-C

Check for Perfect Square in C
Today in this article we will discuss the program to check for perfect square in C programming language. We are given with an integer number and need to print “True” if it is, otherwise “False”.
A perfect square is a number that can be expressed as the product of an integer by itself or as the second exponent of an integer.

Check for Perfect Square or Not
Method 1:
Declare a variable x and set sr = sqrt(x)
Multiply the square root twice.
if(sr*sr==x) return true.
Otherwise return false.
Method 1 :Code in C
Run
#include <stdio.h>
#include <math.h>

int isPerfectSquare(long double x)
{
    if (x >= 0) {
 
        long long sr = sqrt(x);
        return (sr * sr == x);
    }
    
    return 0;
}
 
int main()
{
    long long x = 84;
    if (isPerfectSquare(x)==1)
        printf("True");
    else
        printf("False");
    return 0;
}
Output :
False
Method 2 :
In this method we use the floor and ceil function .
If they are equal that implies the number is a perfect square.
Check for Perfect Square or Not in C
Method 2 :Code in C
Run
#include <stdio.h>
#include <math.h>

void checkperfectsquare(int n)
{
    if (ceil((double)sqrt(n)) == floor((double)sqrt(n))) {
        printf("True");
    }
    else {
        printf("False");
    }
}

int main()
{
 
    int n = 49;
    checkperfectsquare(n);
    return 0;
}
Output :
True
