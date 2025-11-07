# c-programming-
// day 1 code 
/*write a program to input two numbers and display their sum make it look like as begineer has written the coode
*/
#include <stdio.h>

int main()
{
    int num1, num2, sum;

    printf("Enter first number: ");
    scanf("%d", &num1);

    printf("Enter second number: ");
    scanf("%d", &num2);

    sum = num1 + num2;

    printf("The sum is: %d\n", sum);

    return 0;
}
//Write a program to input two numbers and display their sum, difference, product, and quotient.

#include <stdio.h>

int main()
{
    int num1, num2;
    int sum, diff, prod;
    float quotient;

    printf("Enter first number: ");
    scanf("%d", &num1);

    printf("Enter second number: ");
    scanf("%d", &num2);

    sum = num1 + num2;
    diff = num1 - num2;
    prod = num1 * num2;
    quotient = (float)num1 / num2;  // typecast to float for decimal division

    printf("\nResults:\n");
    printf("Sum = %d\n", sum);
    printf("Difference = %d\n", diff);
    printf("Product = %d\n", prod);
    printf("Quotient = %.2f\n", quotient);

    return 0;
}
