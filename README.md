Counting the sum of numbers in a string.
In this article we will learn how to code a C program to count the sum of numbers in a string. To do this we will be using a for loop that will iterate each character of the string and check if the character iterated is a numeric value or not. And if it is found to be a numeric value then we will add that value into the variable that we have assigned to store the sum of the numbers.

C program to count the sum of numbers in a string
Algorithm:
Initialize the variables.
Accept the input.
Initialize a for loop and terminate it at the end of string. 
Iterate each character of the string through that loop.
If the character iterated is a numeric value then we will add that value.
Print result.
C programming code to count the sum of numbers is a string.
#include<stdio.h>  
int main()
{
    //Initializing variables.
    char str[100] = "4PREP2INSTA6";
    int i,sum = 0;
    
    //Iterating each character through for loop.
    for (i= 0; str[i] != '\0'; i++)
    {
        if ((str[i] >= '0') && (str[i] <= '9'))  //Checking for numeric characters.
        {
            
            sum += (str[i] - '0'); //Adding numeric characters.

        }
    }
    //Printing result.
    printf("Sum of all digits:\n%d", sum);
    return 0; 
}
Output

Sum of all digits:
12
