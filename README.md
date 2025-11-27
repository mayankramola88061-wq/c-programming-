# c-programming-


DAY 1 code 

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
DAY - 2 code
// Write a program to calculate the area and perimeter of a rectangle given its length and breadth.

    #include <stdio.h>

    int main() {
         float length, breadth, area, perimeter;

    // Input
    printf("Enter length of the rectangle: ");
    scanf("%f", &length);

    printf("Enter breadth of the rectangle: ");
    scanf("%f", &breadth);

    // Calculations
    area = length * breadth;
    perimeter = 2 * (length + breadth);

    // Output
    printf("\nArea of the rectangle = %.2f\n", area);
    printf("Perimeter of the rectangle = %.2f\n", perimeter);

    return 0;
    }


//Write a program to calculate the area and perimeter of a rectangle given its length and breadth.

    #include <stdio.h>

    int main() {
        float radius, area, circumference;
        float pi = 3.14159;

    printf("Enter the radius of the circle: ");
    scanf("%f", &radius);

    area = pi * radius * radius;
    circumference = 2 * pi * radius;

    printf("Area of the circle = %.2f\n", area);
    printf("Circumference of the circle = %.2f\n", circumference);

    return 0;
    }

DAY 3 code 

 //Write a program to convert temperature from Celsius to Fahrenheit.
 
    #include <stdio.h>

    int main() {
        float celsius, fahrenheit;

    printf("Enter temperature in Celsius: ");
    scanf("%f", &celsius);

    fahrenheit = (celsius * 9.0 / 5.0) + 32;

    printf("Temperature in Fahrenheit = %.2f\n", fahrenheit);

    return 0;
    }

//Write a program to swap two numbers using a third variable.

    #include <stdio.h>

    int main() {
        int a, b, temp;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    printf("Before swapping: a = %d, b = %d\n", a, b);

    // Swapping using a third variable
    temp = a;
    a = b;
    b = temp;

    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;
    }

DAY - 4 

//Write a program to swap two numbers without using a third variable.


    #include <stdio.h>

    int main() {
         int a, b;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    printf("Before swapping: a = %d, b = %d\n", a, b);

    // Swapping without using a third variable
    a = a + b;
    b = a - b;
    a = a - b;

    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;
    }

//Write a program to find and display the sum of the first n natural numbers.

    #include <stdio.h>

    int main() {
          int n, sum;

    printf("Enter the value of n: ");
    scanf("%d", &n);

    sum = n * (n + 1) / 2;

    printf("Sum of first %d natural numbers = %d\n", n, sum);

    return 0;
    }

DAY - 5

 //Write a program to calculate simple and compound interest for given principal, rate, and time.


    #include <stdio.h>
    #include <math.h>

    int main() {
        float principal, rate, time, SI, CI, amount;

        printf("Enter Principal: ");
        scanf("%f", &principal);

        printf("Enter Rate of Interest: ");
        scanf("%f", &rate);

        printf("Enter Time in years: ");
        scanf("%f", &time);

        // Simple Interest
        SI = (principal * rate * time) / 100;

        // Compound Interest
         amount = principal * pow((1 + rate / 100), time);
        CI = amount - principal;

        printf("Simple Interest = %.2f\n", SI);
        printf("Compound Interest = %.2f\n", CI);

        return 0;
        }

//Write a program to input time in seconds and convert it to hours:minutes:seconds format.

    #include <stdio.h>

    int main() {
        int total_seconds, hours, minutes, seconds;

        printf("Enter time in seconds: ");
        scanf("%d", &total_seconds);

        hours = total_seconds / 3600;            // 1 hour = 3600 seconds
        minutes = (total_seconds % 3600) / 60;   // remaining minutes
        seconds = total_seconds % 60;            // remaining seconds

        printf("Time = %02d:%02d:%02d\n", hours, minutes, seconds);

        return 0;
        }

DAY-6

   //Write a program to input an integer and check whether it is even or odd using if–else.

    #include <stdio.h>

    int main() {
        int num;

        printf("Enter an integer: ");
        scanf("%d", &num);

        if (num % 2 == 0) {
            printf("%d is Even\n", num);
        } else {
            printf("%d is Odd\n", num);
        }

        return 0;
        }
        
  //Write a program to input an integer and check whether it is positive, negative or zero using nested if–else.

#include <stdio.h>

int main() {
    int num;

    printf("Enter an integer: ");
    scanf("%d", &num);

    if (num >= 0) {              // Outer if
        if (num == 0) {          // Nested if
            printf("The number is Zero\n");
        } else {
            printf("The number is Positive\n");
        }
    } else {
        printf("The number is Negative\n");
    }

    return 0;
}

DAY-7 

  //Write a program to input a year and check whether it is a leap year or not using conditional statements.

#include <stdio.h>

int main() {
    int year;

    printf("Enter a year: ");
    scanf("%d", &year);

    if (year % 400 == 0) {
        printf("%d is a Leap Year\n", year);
    }
    else if (year % 100 == 0) {
        printf("%d is Not a Leap Year\n", year);
    }
    else if (year % 4 == 0) {
        printf("%d is a Leap Year\n", year);
    }
    else {
        printf("%d is Not a Leap Year\n", year);
    }

    return 0;
}

//Write a program to input a character and check whether it is a vowel or consonant using if–else.

#include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf("%c", &ch);

    // Check for vowel
    if (ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u' ||
        ch=='A' || ch=='E' || ch=='I' || ch=='O' || ch=='U') {
        
        printf("%c is a Vowel\n",
        
DAY-8 
   //Write a program to input a character and check whether it is an uppercase alphabet, lowercase alphabet, digit, or special character.
  #include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf("%c", &ch);

    if (ch >= 'A' && ch <= 'Z') {
        printf("%c is an Uppercase Alphabet\n", ch);
    }
    else if (ch >= 'a' && ch <= 'z') {
        printf("%c is a Lowercase Alphabet\n", ch);
    }
    else if (ch >= '0' && ch <= '9') {
        printf("%c is a Digit\n", ch);
    }
    else {
        printf("%c is a Special Character\n", ch);
    }

    return 0;
}

//Write a program to input three numbers and find the largest among them using if–else.

#include <stdio.h>

int main() {
    int a, b, c;

    printf("Enter three numbers: ");
    scanf("%d %d %d", &a, &b, &c);

    if (a >= b && a >= c) {
        printf("%d is the largest\n", a);
    }
    else if (b >= a && b >= c) {
        printf("%d is the largest\n", b);
    }
    else {
        printf("%d is

DAY -9

//Write a program to find the roots of a quadratic equation and categorize them.

#include <stdio.h>
#include <math.h>

int main() {
    float a, b, c, D, root1, root2, realPart, imagPart;

    printf("Enter coefficients a, b and c: ");
    scanf("%f %f %f", &a, &b, &c);

    D = b*b - 4*a*c;  // Discriminant

    if (D > 0) {
        // Real and distinct roots
        root1 = (-b + sqrt(D)) / (2 * a);
        root2 = (-b - sqrt(D)) / (2 * a);
        printf("Roots are Real and Distinct.\n");
        printf("Root 1 = %.2f\n", root1);
        printf("Root 2 = %.2f\n", root2);
    }
    else if (D == 0) {
        // Real and equal roots
        root1 = root2 = -b / (2 * a);
        printf("Roots are Real and Equal.\n");
        printf("Root = %.2f\n", root1);
    }
    else {
        // Imaginary roots
        realPart = -b / (2 * a);
        imagPart = sqrt(-D) / (2 * a);
        printf("Roots are Imaginary (Complex).\n");
        printf("Root 1 = %.2f + %.2fi\n", realPart, imagPart);
        printf("Root 2 = %.2f - %.2fi\n", realPart, imagPart);
    }

    return 0;
}

//Write a program that accepts a percentage (0-100) and assigns a grade based on the following criteria: 
90-100: Grade A 
80-89: Grade B 
70-79: Grade C 
60-69: Grade D 
below 60: Grade F.

#include <stdio.h>

int main() {
    int percentage;

    printf("Enter your percentage (0-100): ");
    scanf("%d", &percentage);

    if (percentage >= 90 && percentage <= 100) {
        printf("Grade A\n");
    }
    else if (percentage >= 80 && percentage <= 89) {
        printf("Grade B\n");
    }
    else if (percentage >= 70 && percentage <= 79) {
        printf("Grade C\n");
    }
    else if (percentage >= 60 && percentage <= 69) {
        printf("Grade D\n");
    }
    else if (percentage >= 0 && percentage < 60) {
        printf("Grade F\n");
    }
    else {
        printf("Invalid percentage! Please enter a value between 0 and 100.\n");
    }

    return 0;
}

DAy-10 
    //Write a program to classify a triangle as Equilateral, Isosceles, or Scalene based on its side lengths.

    #include <stdio.h>

int main() {
    int a, b, c;

    printf("Enter the three sides of the triangle: ");
    scanf("%d %d %d", &a, &b, &c);

    // Check if the sides form a valid triangle
    if (a + b > c && a + c > b && b + c > a) {

        if (a == b && b == c) {
            printf("Equilateral Triangle\n");
        }
        else if (a == b || b == c || a == c) {
            printf("Isosceles Triangle\n");
        }
        else {
            printf("Scalene Triangle\n");
        }

    } else {
        printf("The given sides do not form a valid triangle.\n");
    }

    return 0;
}

//Write a program to display the day of the week based on a number (1–7) using switch-case.

#include <stdio.h>

int main() {
    int day;

    printf("Enter a number (1-7): ");
    scanf("%d", &day);

    switch(day) {
        case 1:
            printf("Monday\n");
            break;
        case 2:
            printf("Tuesday\n");
            break;
        case 3:
            printf("Wednesday\n");
            break;
        case 4:
            printf("Thursday\n");
            break;
        case 5:
            printf("Friday\n");
            break;
        case 6:
            printf("Saturday\n");
            break;
        case 7:
            printf("Sunday\n");
            break;
        default:
            printf("Invalid number! Please enter between 1 and 7.\n");
    }

    return 0;
}

DAY-11 
 //Write a program to display the month name and number of days using switch-case for a given month number.
#include <stdio.h>

int main() {
    int month;

    printf("Enter month number (1-12): ");
    scanf("%d", &month);

    switch(month) {
        case 1:
            printf("January - 31 days\n");

//Write a program to find profit or loss percentage given cost price and selling price.

#include <stdio.h>

int main() {
    float cp, sp, profit, loss, percent;

    printf("Enter Cost Price: ");
    scanf("%f", &cp);

    printf("Enter Selling Price: ");
    scanf("%f", &sp);

    if (sp > cp) {
        profit = sp - cp;
        percent = (profit / cp) * 100;
        printf("Profit = %.2f\n", profit);
        printf("Profit Percentage = %.2f%%\n", percent);
    }
    else if (cp > sp) {
        loss = cp - sp;
        percent = (loss / cp) * 100;
        printf("Loss = %.2f\n", loss);
        printf("Loss Percentage = %.2f%%\n", percent);
    }
    else {
        printf("No Profit, No Loss.\n");
    }

    return 0;
}

DAY-12

 //Write a program to calculate library fine based on late days as follows: 
First 5 days late: ₹2/day 
Next 5 days late: ₹4/day 
Next 20 days days late: ₹6/day 
More than 30 days: Membership Cancelled

#include <stdio.h>

int main() {
    int days;
    int fine = 0;

    printf("Enter number of days late: ");
    scanf("%d", &days);

    if (days <= 0) {
        printf("No fine.\n");
    }
    else if (days <= 5) {
        fine = days * 2;
        printf("Fine = ₹%d\n", fine);
    }
    else if (days <= 10) {
        fine = (5 * 2) + (days - 5) * 4;
        printf("Fine = ₹%d\n", fine);
    }
    else if (days <= 30) {
        fine = (5 * 2) + (5 * 4) + (days - 10) * 6;
        printf("Fine = ₹%d\n", fine);
    }
    else {
        printf("Membership Cancelled\n");
    }

    return 0;
}

//Write a program to calculate electricity bill based on units consumed with these rates: 
First 100 units at ₹5/unit 
Next 100 units at ₹7/unit 
Next 100 units at ₹10/unit 
Above at ₹12/unit           

#include <stdio.h>

int main() {
    int units;
    float bill = 0;

    printf("Enter electricity units consumed: ");
    scanf("%d", &units);

    if (units <= 0) {
        printf("Invalid units.\n");
    }
    else if (units <= 100) {
        bill = units * 5;
    }
    else if (units <= 200) {
        bill = (100 * 5) + (units - 100) * 7;
    }
    else if (units <= 300) {
        bill = (100 * 5) + (100 * 7) + (units - 200) * 10;
    }
    else {
        bill = (100 * 5) + (100 * 7) + (100 * 10) + (units - 300) * 12;
    }

    printf("Total Electricity Bill = ₹%.2f\n", bill);

    return 0;
}
DAY-13 
//Write a program to implement a basic calculator using switch-case for +, -, *, /, %.


#include <stdio.h>

int main() {
    int a, b;
    char op;

    printf("Enter first number: ");
    scanf("%d", &a);

    printf("Enter second number: ");
    scanf("%d", &b);

    printf("Enter operator (+, -, *, /, %%): ");
    scanf(" %c", &op);   // space before %c to avoid input issues

    switch(op) {
        case '+':
            printf("Result = %d\n", a + b);
            break;

        case '-':
            printf("Result = %d\n", a - b);
            break;

        case '*':
            printf("Result = %d\n", a * b);
            break;

        case '/':
            if (b == 0)
                printf("Error: Division by zero not allowed.\n");
            else
                printf("Result = %d\n", a / b);
            break;

        case '%':
            if (b == 0)
                printf("Error: Modulo by zero not allowed.\n");
            else
                printf("Result = %d\n", a % b);
            break;

        default:
            printf("Invalid operator.\n");
    }

    return 0;
}

//Write a program to print numbers from 1 to n.

#include <stdio.h>

int main() {
    int n;

    printf("Enter value of n: ");
    scanf("%d", &n);

    printf("Numbers from 1 to %d:\n", n);

    for (int i = 1; i <= n; i++) {
        printf("%d ", i);
    }

    return 0;
}
DAY-14
//Write a program to print the sum of the first n odd numbers.


#include <stdio.h>

int main() {
    int n, sum = 0;

    printf("Enter value of n: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        sum += (2 * i - 1);   // i-th odd number
    }

    printf("Sum of first %d odd numbers = %d\n", n, sum);

    return 0;
}


//Write a program to print the product of even numbers from 1 to n.

#include <stdio.h>

int main() {
    int n;
    long long product = 1;   // use long long to store large values

    printf("Enter value of n: ");
    scanf("%d", &n);

    for (int i = 2; i <= n; i += 2) {   // iterate only even numbers
        product *= i;
    }

    printf("Product of even numbers from 1 to %d = %lld\n", n, product);

    return 0;
}

DAY-15 
//Write a program to calculate the factorial of a number.

#include <stdio.h>

int main() {
    int n;
    long long fact = 1;

    printf("Enter a number: ");
    scanf("%d", &n);

    if (n < 0) {
        printf("Factorial of a negative number doesn't exist.\n");
        return 0;
    }

    for (int i = 1; i <= n; i++) {
        fact *= i;
    }

    printf("Factorial of %d = %lld\n", n, fact);

    return 0;
}

//Write a program to reverse a given number.

#include <stdio.h>

int main() {
    int n, reversed = 0, digit;

    printf("Enter a number: ");
    scanf("%d", &n);

    while (n != 0) {
        digit = n % 10;            // extract last digit
        reversed = reversed * 10 + digit;   // build reversed number
        n = n / 10;                // remove last digit
    }

    printf("Reversed number = %d\n", reversed);

    return 0;
}

DAY-16
//Write a program to take a number as input and print its equivalent binary representation.

#include <stdio.h>

int main() {
    int n, binary[32], i = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    if (n == 0) {
        printf("Binary = 0\n");
        return 0;
    }

    // Convert to binary (store remainders)
    while (n > 0) {
        binary[i] = n % 2;
        n = n / 2;
        i++;
    }

    printf("Binary = ");
    // Print in reverse order
    for (int j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }

    printf("\n");
    return 0;
}

//Write a program to check if a number is a palindrome.

#include <stdio.h>

int main() {
    int n, original, reversed = 0, digit;

    printf("Enter a number: ");
    scanf("%d", &n);

    original = n;  // store original number

    while (n != 0) {
        digit = n % 10;               // get last digit
        reversed = reversed * 10 + digit;  // build reverse
        n = n / 10;                   // remove last digit
    }

    if (original == reversed)
        printf("The number is a Palindrome.\n");
    else
        printf("The number is NOT a Palindrome.\n");

    return 0;
}

DAY-17
//Write a program to check if a number is an Armstrong number.

#include <stdio.h>
#include <math.h>

int main() {
    int n, original, digit, count = 0;
    double sum = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    original = n;

    // Step 1: Count digits
    int temp = n;
    while (temp != 0) {
        temp /= 10;
        count++;
    }

    // Step 2: Calculate sum of digits raised to power count
    temp = n;
    while (temp != 0) {
        digit = temp % 10;
        sum += pow(digit, count);
        temp /= 10;
    }

    // Step 3: Compare
    if (sum == original)
        printf("%d is an Armstrong number.\n", original);
    else
        printf("%d is NOT an Armstrong number.\n", original);

    return 0;
}

//Write a program to check if a number is prime.

#include <stdio.h>

int main() {
    int n, i, flag = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    if (n <= 1) {
        printf("%d is NOT a prime number.\n", n);
        return 0;
    }

    for (i = 2; i <= n/2; i++) {
        if (n % i == 0) {
            flag = 1;
            brea
        }
    }

    if (flag == 0)
        printf("%d is a prime number.\n", n);
    else
        printf("%d is NOT a prime number.\n", n);

    return 0;
}

DAY-18
//Write a program to print all factors of a given number.

#include <stdio.h>

int main() {
    int n;

    printf("Enter a number: ");
    scanf("%d", &n);

    printf("Factors of %d are: ", n);

    for (int i = 1; i <= n; i++) {
        if (n % i == 0) {
            printf("%d ", i);
        }
    }

    printf("\n");
    return 0;
}

//Write a program to find the HCF (GCD) of two numbers.

#include <stdio.h>

int main() {
    int a, b, hcf;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    int min = (a < b) ? a : b;

    for (int i = 1; i <= min; i++) {
        if (a % i == 0 && b % i == 0) {
            hcf = i;
        }
    }

    printf("HCF (GCD) of %d and %d = %d\n", a, b, hcf);

    return 0;
}
DAY-19

//Write a program to find the LCM of two numbers.

#include <stdio.h>

int main() {
    int a, b, hcf = 1, lcm;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    int min = (a < b) ? a : b;

    // Find HCF
    for (int i = 1; i <= min; i++) {
        if (a % i == 0 && b % i == 0) {
            hcf = i;
        }
    }

    // Calculate LCM
    lcm = (a * b) / hcf;

    printf("LCM of %d and %d = %d\n", a, b, lcm);

    return 0;
}

//Write a program to find the sum of digits of a number.

#include <stdio.h>

int main() {
    int n, sum = 0, digit;

    printf("Enter a number: ");
    scanf("%d", &n);

    while (n > 0) {
        digit = n % 10;   // extract last digit
        sum += digit;     // add to sum
        n = n / 10;       // remove last digit
    }

    printf("Sum of digits = %d\n", sum);

    return 0;
}

DAY-20
//Write a program to find the product of odd digits of a number.

#include <stdio.h>

int main() {
    int n, digit;
    int product = 1;
    int foundOdd = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    while (n > 0) {
        digit = n % 10;

        if (digit % 2 == 1) {   // check odd digit
            product *= digit;
            foundOdd = 1;
        }

        n /= 10;
    }

    if (foundOdd)
        printf("Product of odd digits = %d\n", product);
    else
        printf("No odd digits present.\n");

    return 0;
}

//Write a program to find the 1’s complement of a binary number and print it.

#include <stdio.h>

int main() {
    char binary[100];

    printf("Enter a binary number: ");
    scanf("%s", binary);

    // Convert each bit to its 1's complement
    for (int i = 0; binary[i] != '\0'; i++) {
        if (binary[i] == '0')
            binary[i] = '1';
        else if (binary[i] == '1')
            binary[i] = '0';
        else {
            printf("Invalid binary number.\n");
            return 0;
        }
    }

    printf("1's Complement = %s\n", binary);

    return 0;
}

DAY-21
//Write a program to swap the first and last digit of a number.

#include <stdio.h>
#include <math.h>

int main() {
    int n, first, last, digits, power, middle;

    printf("Enter a number: ");
    scanf("%d", &n);

    last = n % 10;                 // extract last digit

    digits = (int)log10(n);        // count digits - 1
    power = pow(10, digits);       // 10^(digits)

    first = n / power;             // extract first digit

    middle = n % power;            // remove first digit
    middle = middle / 10;          // remove last digit

    int swapped = last * power + middle * 10 + first;

    printf("Number after swapping first and last digit = %d\n", swapped);

    return 0;
}

//Write a program to check if a number is a perfect number.

#include <stdio.h>

int main() {
    int n, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    // Find sum of proper divisors
    for (int i = 1; i <= n/2; i++) {
        if (n % i == 0) {
            sum += i;
        }
    }

    // Check if perfect
    if (sum == n && n != 0)
        printf("%d is a Perfect Number.\n", n);
    else
        printf("%d is NOT a Perfect Number.\n", n);

    return 0;
}

DAY-22
//Write a program to check if a number is a strong number
#include <stdio.h>

int main() {
    int n, original, digit;
    int sum = 0;

    printf("Enter a number: ");
    scanf("%d", &n);

    original = n;

    while (n > 0) {
        digit = n % 10;

        // find factorial of the digit
        int fact = 1;
        for (int i = 1; i <= digit; i++) {
            fact *= i;
        }

        sum += fact;
        n /= 10;
    }

    if (sum == original)
        printf("%d is a Strong Number.\n", original);
    else
        printf("%d is NOT a Strong Number.\n", original);

    return 0;
}

//Write a program to find the sum of the series: 1 + 3/4 + 5/6 + 7/8 + … up to n terms.

#include <stdio.h>

int main() {
    int n;
    float sum = 0.0;

    printf("Enter number of terms (n): ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        float numerator = 2 * i - 1;     // 1, 3, 5, 7...
        float denominator = 2 * i;       // 2, 4, 6, 8...
        sum += numerator / denominator;
    }

    printf("Sum of the series = %.4f\n", sum);

    return 0;
}

DAY-23
//Write a program to find the sum of the series: 2/3 + 4/7 + 6/11 + 8/15 + ... up to n terms.

#include <stdio.h>

int main() {
    int n;
    float sum = 0.0;

    printf("Enter number of terms (n): ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++) {
        float numerator = 2 * i;         // 2, 4, 6, 8, ...
        float denominator = 4 * i - 1;   // 3, 7, 11, 15, ...
        sum += numerator / denominator;
    }

    printf("Sum of the series = %.4f\n", sum);

    return 0;
}

//Write a program to print the following pattern:
*****
*****
*****
*****
*****

#include <stdio.h>

int main() {
    for (int i = 1; i <= 5; i++) {        // 5 rows
        for (int j = 1; j <= 5; j++) {    // 5 columns
            printf("*");
        }
        printf("\n");
    }

    return 0;
}

DAY-24
//Write a program to print the following pattern:
*
**
***
****
*****

#include <stdio.h>

int main() {
    for (int i = 1; i <= 5; i++) {        // number of rows
        for (int j = 1; j <= i; j++) {    // print i stars in each row
            printf("*");
        }
        printf("\n");
    }

    return 0;
}

//Write a program to print the following pattern:
1
12
123
1234
12345

#include <stdio.h>

int main() {
    for (int i = 1; i <= 5; i++) {          // rows
        for (int j = 1; j <= i; j++) {      // print numbers from 1 to i
            printf("%d", j);
        }
        printf("\n");
    }

    return 0;
}


DAY-25
//Write a program to print the following pattern:
5
45
345
2345
12345

#include <stdio.h>

int main() {
    for (int i = 5; i >= 1; i--) {       // starting number decreases each row
        for (int j = i; j <= 5; j++) {   // print from i up to 5
            printf("%d", j);
        }
        printf("\n");
    }

    return 0;
}

//Write a program to print the following pattern:
*****
 ****
  ***
   **
    *

    #include <stdio.h>

int main() {
    for (int i = 5; i >= 1; i--) {        // number of stars in each row
        for (int s = 0; s < 5 - i; s++) { // print spaces
            printf(" ");
        }
        for (int j = 1; j <= i; j++) {    // print stars
            printf("*");
        }
        printf("\n");
    }

    return 0;
}

DAY-26
//Write a program to print the following pattern:
    5
   45
  345
 2345
12345

#include <stdio.h>

int main() {
    for (int i = 5; i >= 1; i--) {

        // print spaces
        for (int s = 1; s < i; s++) {
            printf(" ");
        }

        // print numbers from i to 5
        for (int j = i; j <= 5; j++) {
            printf("%d", j);
        }

        printf("\n");
    }

    return 0;
}

//Write a program to print the following pattern:

*

*
*
*

*
*
*
*
*

*
*
*

*

#include <stdio.h>

int main() {
    int pattern[] = {1, 3, 5, 3, 1};

    for (int i = 0; i < 5; i++) {

        // print stars for this block
        for (int j = 0; j < pattern[i]; j++) {
            printf("*\n");
        }

        // print a blank line between blocks (except last)
        if (i != 4)
            printf("\n");
    }

    return 0;
}

DAY-27
//Write a program to print the following pattern:
*
***
*****
*******
*********
*******
*****
***
*

#include <stdio.h>

int main() {
    int i, j;
    int n = 5;  // middle row has 9 stars → 2*n - 1

    // Upper half
    for (i = 1; i <= n; i++) {
        for (j = 1; j <= 2*i - 1; j++) {
            printf("*");
        }
        printf("\n");
    }

    // Lower half
    for (i = n - 1; i >= 1; i--) {
        for (j = 1; j <= 2*i - 1; j++) {
            printf("*");
        }
        printf("\n");
    }

    return 0;
}

//Write a program to print the following pattern:

   *
  ***
 *****
*******
 *****
  ***
   *

   #include <stdio.h>

int main() {
    int i, j;
    int n = 4; // middle row has 7 stars → 2*n - 1 = 7

    // Upper half
    for (i = 1; i <= n; i++) {

        // print spaces
        for (j = 1; j <= n - i; j++) {
            printf(" ");
        }

        // print stars
        for (j = 1; j <= 2*i - 1; j++) {
            printf("*");
        }

        printf("\n");
    }

    // Lower half
    for (i = n - 1; i >= 1; i--) {

        // print spaces
        for (j = 1; j <= n - i; j++) {
            printf(" ");
        }

        // print stars
        for (j = 1; j <= 2*i - 1; j++) {
            printf("*");
        }

        printf("\n");
    }

    return 0;
}

DAY-28
//Write a program to print all the prime numbers from 1 to n.

#include <stdio.h>

int main() {
    int n, i, j, isPrime;

    printf("Enter value of n: ");
    scanf("%d", &n);

    printf("Prime numbers from 1 to %d are:\n", n);

    for (i = 2; i <= n; i++) {   // start from 2 (1 is not prime)
        isPrime = 1;             // assume i is prime

        for (j = 2; j <= i / 2; j++) {
            if (i % j == 0) {
                isPrime = 0;     // not prime
                break;
            }
        }

        if (isPrime == 1) {
            printf("%d ", i);
        }
    }

    return 0;
}
//Read and print elements of a one-dimensional array.

#include <stdio.h>

int main() {
    int n;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    // Read array elements
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Print array elements
    printf("Array elements are:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
DAY-29 
//Find the sum of array elements.

#include <stdio.h>

int main() {
    int n, sum = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        sum += arr[i];   // add each element to sum
    }

    printf("Sum of array elements = %d\n", sum);

    return 0;
}

//Find the maximum and minimum element in an array.

#include <stdio.h>

int main() {
    int n;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int max = arr[0];
    int min = arr[0];

    for (int i = 1; i < n; i++) {
        if (arr[i] > max)
            max = arr[i];

        if (arr[i] < min)
            min = arr[i];
    }

    printf("Maximum element = %d\n", max);
    printf("Minimum element = %d\n", min);

    return 0;
}
DAY-30

//Count even and odd numbers in an array.

#include <stdio.h>

int main() {
    int n, even = 0, odd = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        if (arr[i] % 2 == 0)
            even++;
        else
            odd++;
    }

    printf("Total even numbers = %d\n", even);
    printf("Total odd numbers = %d\n", odd);

    return 0;
}

//Count positive, negative, and zero elements in an array.


#include <stdio.h>

int main() {
    int n, pos = 0, neg = 0, zero = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);

        if (arr[i] > 0)
            pos++;
        else if (arr[i] < 0)
            neg++;
        else
            zero++;
    }

    printf("Positive elements = %d\n", pos);
    printf("Negative elements = %d\n", neg);
    printf("Zero elements = %d\n", zero);

    return 0;
}

DAY-31
//Search for an element in an array using linear search.

#include <stdio.h>

int main() {
    int n, key, found = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter element to search: ");
    scanf("%d", &key);

    for (int i = 0; i < n; i++) {
        if (arr[i] == key) {
            printf("Element found at position %d\n", i + 1);
            found = 1;
            break;
        }
    }

    if (!found) {
        printf("Element not found in the array.\n");
    }

    return 0;
}

//Reverse an array without taking extra space.
#include <stdio.h>

int main() {
    int n;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Reverse the array in-place
    int start = 0, end = n - 1;
    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;

        start++;
        end--;
    }

    printf("Reversed array:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
DAY-31
//Merge two arrays.

#include <stdio.h>

int main() {
    int n, key, found = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter element to search: ");
    scanf("%d", &key);

    // Linear search
    for (int i = 0; i < n; i++) {
        if (arr[i] == key) {
//Reverse an array without taking extra space.#include <stdio.h>

#include <stdio.h>

int main() {
    int n;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // In-place reversal using two pointers
    int start = 0, end = n - 1;

    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;

        start++;
        end--;
    }

    printf("Reversed array:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
DAY-32
//Merge two arrays.
int main() {
    int n1, n2;

    printf("Enter size of first array: ");
    scanf("%d", &n1);

    int arr1[n1];
    printf("Enter %d elements of first array:\n", n1);
    for (int i = 0; i < n1; i++) {
        scanf("%d", &arr1[i]);
    }

    printf("Enter size of second array: ");
    scanf("%d", &n2);

    int arr2[n2];
    printf("Enter %d elements of second array:\n", n2);
    for (int i = 0; i < n2; i++) {
        scanf("%d", &arr2[i]);
    }

    int merged[n1 + n2];

    // Copy arr1 into merged
    for (int i = 0; i < n1; i++) {
        merged[i] = arr1[i];
    }

    // Copy arr2 into merged
    for (int i = 0; i < n2; i++) {
        merged[n1 + i] = arr2[i];
    }

    printf("Merged array:\n");
    for (int i = 0; i < n1 + n2; i++) {
        printf("%d ", merged[i]);
    }

    return 0;
}

DAY-32
//Merge two arrays.

#include <stdio.h>

int main() {
    int n1, n2;

    printf("Enter size of first array: ");
    scanf("%d", &n1);

    int arr1[n1];
    printf("Enter %d elements of first array:\n", n1);
    for (int i = 0; i < n1; i++) {
        scanf("%d", &arr1[i]);
    }

    printf("Enter size of second array: ");
    scanf("%d", &n2);

    int arr2[n2];
    printf("Enter %d elements of second array:\n", n2);
    for (int i = 0; i < n2; i++) {
        scanf("%d", &arr2[i]);
    }

    int merged[n1 + n2];

    // Copy arr1 into merged
    for (int i = 0; i < n1; i++) {
        merged[i] = arr1[i];
    }

    // Copy arr2 into merged
    for (int i = 0; i < n2; i++) {
        merged[n1 + i] = arr2[i];
    }

    printf("Merged array:\n");
    for (int i = 0; i < n1 + n2; i++) {
        printf("%d ", merged[i]);
    }

    return 0;
}
//Find the digit that occurs the most times in an integer number.

#include <stdio.h>

int main() {
    long long n;
    int freq[10] = {0};  // frequency of digits 0–9
    int digit;

    printf("Enter an integer number: ");
    scanf("%lld", &n);

    // If number is negative, make it positive
    if (n < 0)
        n = -n;

    // Count digit frequencies
    while (n > 0) {
        digit = n % 10;
        freq[digit]++;
        n /= 10;
    }

    // Find digit with highest frequency
    int maxDigit = 0;
    int maxFreq = freq[0];

    for (int i = 1; i < 10; i++) {
        if (freq[i] > maxFreq) {
            maxFreq = freq[i];
            maxDigit = i;
        }
    }

    printf("Digit occurring most times = %d\n", maxDigit);
    printf("It occurs %d times.\n", maxFreq);

    return 0;
}
//Find the digit that occurs the most times in an integer number.Search in a sorted array using binary search.

#include <stdio.h>

int main() {
    int n1, n2;

    printf("Enter size of first array: ");
    scanf("%d", &n1);

    int arr1[n1];
    printf("Enter %d elements of first array:\n", n1);
    for (int i = 0; i < n1; i++) {
        scanf("%d", &arr1[i]);
    }

    printf("Enter size of second array: ");
    scanf("%d", &n2);

    int arr2[n2];
    printf("Enter %d elements of second array:\n", n2);
    for (int i = 0; i < n2; i++) {
        scanf("%d", &arr2[i]);
    }

    int merged[n1 + n2];

    // Copy arr1 into merged
    for (int i = 0; i < n1; i++) {
        merged[i] = arr1[i];
    }

    // Copy arr2 after arr1
    for (int i = 0; i < n2; i++) {
        merged[n1 + i] = arr2[i];
    }

    printf("Merged array:\n");
    for (int i = 0; i < n1 + n2; i++) {
        printf("%d ", merged[i]);
    }

    return 0;
}
DAY-33
//Search in a sorted array using binary search.
#include <stdio.h>

int main() {
    int n, key, low, high, mid, found = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements (sorted in ascending order):\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter element to search: ");
    scanf("%d", &key);

    low = 0;
    high = n - 1;

    while (low <= high) {
        mid = (low + high) / 2;

        if (arr[mid] == key) {
            printf("Element found at position %d\n", mid + 1);
            found = 1;
            break;
        }
        else if (arr[mid] < key) {
            low = mid + 1;   // search right half
        }
        else {
            high = mid - 1;  // search left half
        }
    }

    if (!found) {
        printf("Element not found in the array.\n");
    }

    return 0;
}
//#include <stdio.h>

int main() {
    int n, key;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int arr[n + 1];   // extra space for new element

    printf("Enter %d sorted elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter element to insert: ");
    scanf("%d", &key);

    int i = n - 1;

    // Shift elements to the right until correct position is found
    while (i >= 0 && arr[i] > key) {
        arr[i + 1] = arr[i];
        i--;
    }

    // Insert the new element
    arr[i + 1] = key;

    printf("Array after insertion:\n");
    for (int j = 0; j <= n; j++) {
        printf("%d ", arr[j]);
    }

    return 0;
}
DAY-34
//Insert an element in an array at a given position.

#include <stdio.h>

int main() {
    int n, pos, value;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n + 1]; // extra space for new element

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter position and value to insert: ");
    scanf("%d %d", &pos, &value);

    // Shift elements to the right
    for (int i = n; i >= pos; i--) {
        arr[i] = arr[i - 1];
    }

    // Insert element at position (1-based index)
    arr[pos - 1] = value;

    printf("Array after insertion:\n");
    for (int i = 0; i <= n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
//Delete an element from an array.

#include <stdio.h>

int main() {
    int n, pos;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter position to delete: ");
    scanf("%d", &pos);

    // Shift elements left from that position
    for (int i = pos - 1; i < n - 1; i++) {
        arr[i] = arr[i + 1];
    }

    // Print updated array (size becomes n−1)
    printf("Array after deletion:\n");
    for (int i = 0; i < n - 1; i++) {
        printf(
DAY-35
//Find the second largest element in an array.

#include <stdio.h>

int main() {
    int n;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int largest = arr[0];
    int second = -99999999;  // very small number

    // Find largest element
    for (int i = 1; i < n; i++) {
        if (arr[i] > largest) {
            largest = arr[i];
        }
    }

    // Find second largest element
    for (int i = 0; i < n; i++) {
        if (arr[i] > second && arr[i] < largest) {
            second = arr[i];
        }
    }

    printf("%d\n", second);

    return 0;
}
//Rotate an array to the right by k positions.

#include <stdio.h>

int main() {
    int n, k;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter k: ");
    scanf("%d", &k);

    k = k % n; // handle cases where k > n

    // Reverse entire array
    int start = 0, end = n - 1;
    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;
        start++;
        end--;
    }

    // Reverse first k elements
    start = 0;
    end = k - 1;
    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;
        start++;
        end--;
    }

    // Reverse remaining elements
    start = k;
    end = n - 1;
    while (start < end) {
        int temp = arr[start];
        arr[start] = arr[end];
        arr[end] = temp;
        start++;
        end--;
    }

    printf("Rotated array:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}

DAY-36

//Read and print a matrix.

#include <stdio.h>

int main() {
    int rows, cols;

    scanf("%d %d", &rows, &cols);

    int matrix[rows][cols];

    // Read matrix
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            scanf("%d", &matrix[i][j]);
        }
    }

    // Print matrix
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            printf("%d ", matrix[i][j]);
        }
        printf("\n");
    }

    return 0;
}

//Find the sum of all elements in a matrix.

#include <stdio.h>

int main() {
    int rows, cols, sum = 0;

    scanf("%d %d", &rows, &cols);

    int matrix[rows][cols];

    // Read matrix elements
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            scanf("%d", &matrix[i][j]);
            sum += matrix[i][j];
        }
    }

    // Print the sum
    printf("%d", sum);

    return 0;
}
DAY-37
//#include <stdio.h>

int main() {
    int rows, cols;

    scanf("%d %d", &rows, &cols);

    int matrix[rows][cols];
    int rowSum[rows];

    // Read matrix
    for (int i = 0; i < rows; i++) {
        int sum = 0;

        for (int j = 0; j < cols; j++) {
            scanf("%d", &matrix[i][j]);
            sum += matrix[i][j];   // row sum
        }

        rowSum[i] = sum;  // store sum of this row
    }

    // Print row-wise sums
    for (int i = 0; i < rows; i++) {
        printf("%d ", rowSum[i]);
    }

    return 0;
}
//Find the transpose of a matrix.
#include <stdio.h>

int main() {
    int rows, cols;

    scanf("%d %d", &rows, &cols);

    int matrix[rows][cols];
    int transposed[cols][rows];

    // Read the matrix
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            scanf("%d", &matrix[i][j]);
        }
    }

    // Compute transpose
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            transposed[j][i] = matrix[i][j];
        }
    }

    // Print transpose
    for (int i = 0; i < cols; i++) {
        for (int j = 0; j < rows; j++) {
            printf("%d ", transposed[i][j]);
        }
        printf("\n");
    }

    return 0;
}
