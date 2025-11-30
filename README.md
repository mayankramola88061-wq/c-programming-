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
//

    #include <stdio.h>

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
//
   #include <stdio.h>

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
DAY- 38

//Add two matrices.

    #include <stdio.h>

    int main() {
        int r, c;

    printf("Enter number of rows: ");
    scanf("%d", &r);

    printf("Enter number of columns: ");
    scanf("%d", &c);

    int A[r][c], B[r][c], Sum[r][c];

    printf("Enter elements of Matrix A:\n");
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            scanf("%d", &A[i][j]);
        }
    }

    printf("Enter elements of Matrix B:\n");
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            scanf("%d", &B[i][j]);
        }
    }

    // Add matrices
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            Sum[i][j] = A[i][j] + B[i][j];
        }
    }

    printf("Sum of the two matrices:\n");
    for (int i = 0; i < r; i++) {
        for (int j = 0; j < c; j++) {
            printf("%d ", Sum[i][j]);
        }
        printf("\n");
    }

    return 0;
    }

//Check if a matrix is symmetric.

    #include <stdio.h>

    int main() {
        int n;

    printf("Enter the size of the square matrix (n x n): ");
    scanf("%d", &n);

    int a[n][n];

    // Read matrix
    printf("Enter the elements of the matrix:\n");
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Check symmetric
    int symmetric = 1;  // assume true
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            if (a[i][j] != a[j][i]) {
                symmetric = 0;
                break;
            }
        }
    }

    if (symmetric)
        printf("The matrix is symmetric.\n");
    else
        printf("The matrix is not symmetric.\n");

    return 0;
    }

DAY-39
//Check if the elements on the diagonal of a matrix are distinct.

    include <stdio.h>

    int main() {
        int n;

    printf("Enter the size of the square matrix: ");
    scanf("%d", &n);

    int a[n][n];

    printf("Enter the elements of the matrix:\n");
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    // Check distinct diagonal elements
    int distinct = 1;  // assume distinct unless found same

    for (int i = 0; i < n; i++) {
        for (int j = i + 1; j < n; j++) {
            if (a[i][i] == a[j][j]) {
                distinct = 0;
                break;
            }
        }
        if (!distinct)
            break;
    }

    if (distinct)
        printf("Diagonal elements are distinct.\n");
    else
        printf("Diagonal elements are NOT distinct.\n");

    return 0;
    }
//Find the sum of main diagonal elements for a square matrix.

    #include <stdio.h>

    int main() {
        int n;

    printf("Enter the size of the square matrix: ");
    scanf("%d", &n);

    int mat[n][n];

    printf("Enter the elements of the matrix:\n");
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            scanf("%d", &mat[i][j]);
        }
    }

    int sum = 0;

    for (int i = 0; i < n; i++) {
        sum += mat[i][i];  // main diagonal element
    }

    printf("Sum of main diagonal elements = %d\n", sum);

    return 0;
    }

DAY-40

//Perform diagonal traversal of a matrix.
#include <stdio.h>

    int main() {
        int n;

    printf("Enter the size of square matrix: ");
    scanf("%d", &n);

    int a[n][n];

    printf("Enter matrix elements:\n");
    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    printf("Diagonal Traversal:\n");

    // Print diagonals starting from first row
    for (int col = 0; col < n; col++) {
        int i = 0, j = col;
        while (i < n && j >= 0) {
            printf("%d ", a[i][j]);
            i++;
            j--;
        }
        printf("\n");
    }

    // Print diagonals starting from last column except top element
    for (int row = 1; row < n; row++) {
        int i = row, j = n - 1;
        while (i < n && j >= 0) {
            printf("%d ", a[i][j]);
            i++;
            j--;
        }
        printf("\n");
    }

    return 0;
    }

//Multiply two matrices.

    #include <stdio.h>

    int main() {
        int r1, c1, r2, c2;

    // Read dimensions of first matrix
    printf("Enter rows and columns of first matrix: ");
    scanf("%d %d", &r1, &c1
    );

    // Read dimensions of second matrix
    printf("Enter rows and columns of second matrix: ");
    scanf("%d %d", &r2, &c2);

    // Check matrix multiplication condition
    if (c1 != r2) {
        printf("Matrix multiplication not possible.\n");
        return 0;
    }

    int A[r1][c1], B[r2][c2], C[r1][c2];

    // Input for first matrix
    printf("Enter elements of first matrix:\n");
    for (int i = 0; i < r1; i++) {
        for (int j = 0; j < c1; j++) {
            scanf("%d", &A[i][j]);
        }
    }

    // Input for second matrix
    printf("Enter elements of second matrix:\n");
    for (int i = 0; i < r2; i++) {
        for (int j = 0; j < c2; j++) {
            scanf("%d", &B[i][j]);
        }
    }

    // Initialize result matrix with 0
    for (int i = 0; i < r1; i++) {
        for (int j = 0; j < c2; j++) {
            C[i][j] = 0;
        }
    }

    // Matrix multiplication
    for (int i = 0; i < r1; i++) {
        for (int j = 0; j < c2; j++) {
            for (int k = 0; k < c1; k++) {
                C[i][j] += A[i][k] * B[k][j];
            }
        }
    }

    // Print result matrix
    printf("Resultant matrix:\n"
    
DAY-41
//Count characters in a string without using built-in length functions.

    #include <stdio.h>

    int main() {
        char str[100];
        int count = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Count characters manually
    for (int i = 0; str[i] != '\0'; i++) {
        count++;
    }

    // Excluding the newline character added by fgets (optional)
    if (str[count - 1] == '\n') {
        count--;
    }

    printf("Total characters = %d\n", count);

    return 0;
    }
//Print each character of a string on a new line.

    #include <stdio.h>

    int main() {
        char str[100];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Print each character on a new line
    for (int i = 0; str[i] != '\0'; i++) {
        printf("%c\n", str[i]);
    }

    return 0;
    }
DAY-42 
//Count vowels and consonants in a string.

    #include <stdio.h>

    int main() {
    char str[100];
    int i, vowels = 0, consonants = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for (i = 0; str[i] != '\0'; i++) {
        char c = str[i];

        // Check lowercase and uppercase vowels
        if (c=='A' || c=='E' || c=='I' || c=='O' || c=='U' ||
            c=='a' || c=='e' || c=='i' || c=='o' || c=='u') {
            vowels++;
        }
        else if ((c >= 'A' && c <= 'Z') || (c >= 'a' && c <= 'z')) {
            // Any alphabet that is not a vowel is a consonant
            consonants++;
        }
    }

    printf("Vowels: %d\n", vowels);
    printf("Consonants: %d\n", consonants);

    return 0;
    }
//Convert a lowercase string to uppercase without using built-in functions.

    #include <stdio.h>

    int main() {
        char str[100];

    printf("Enter a lowercase string: ");
    fgets(str, sizeof(str), stdin);

    // Convert to uppercase manually
    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] >= 'a' && str[i] <= 'z') {
            str[i] = str[i] - 32; // ASCII conversion
        }
    }

    printf("Uppercase string: %s", str);
    return 0;
    }
DAY-43
//Reverse a string.

    #include <stdio.h>

    int main() {
        char str[100];
        int i, len = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Find length manually
    while (str[len] != '\0' && str[len] != '\n') {
        len++;
    }

    // Reverse and print
    printf("Reversed string: ");
    for (i = len - 1; i >= 0; i--) {
        printf("%c", str[i]);
    }

    return 0;
    }
//Check if a string is a palindrome.

    #include <stdio.h>

    int main() {
       char str[100];
       int i, j, flag = 1;

    printf("Enter a string: ");
    scanf("%s", str);

    // Set pointers i (start) and j (end)
    for (i = 0; str[i] != '\0'; i++);
    j = i - 1;

    // Compare characters from both ends
    for (i = 0; i < j; i++, j--) {
        if (str[i] != str[j]) {
            flag = 0;
            break;
        }
    }

    if (flag)
        printf("The string is a palindrome.\n");
    else
        printf("The string is not a palindrome.\n");

    return 0;
    }
DAY-44
//Count spaces, digits, and special characters in a string.

    #include <stdio.h>

    int main() {
        char str[200];
        int spaces = 0, digits = 0, special = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] == ' ')
            spaces++;
        else if (str[i] >= '0' && str[i] <= '9')
            digits++;
        else if ((str[i] >= 'A' && str[i] <= 'Z') ||
                 (str[i] >= 'a' && str[i] <= 'z'))
            continue; // letters are ignored
        else
            special++;
    }

    printf("Spaces: %d\n", spaces);
    printf("Digits: %d\n", digits);
    printf("Special characters: %d\n", special);

    return 0;
    }
//Replace spaces with hyphens in a string.

    #include <stdio.h>

    int main() {
        char str[200];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] == ' ')
            str[i] = '-';
    }

    printf("String after replacing spaces: %s", str);

    return 0;
    }

DAY-45

//Count frequency of a given character in a string.

    #include <stdio.h>

    int main() {
        char str[100], ch;
        int count = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    printf("Enter the character to count: ");
    scanf("%c", &ch);

    // Count frequency
    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] == ch) {
            count++;
        }
    }

    printf("Frequency of '%c' = %d\n", ch, count);

    return 0;
    }

//Toggle case of each character in a string.

    #include <stdio.h>

    int main() {
        char str[100];

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] >= 'a' && str[i] <= 'z') {
            str[i] = str[i] - 32; // convert lowercase → uppercase
        }
        else if (str[i] >= 'A' && str[i] <= 'Z') {
            str[i] = str[i] + 32; // convert uppercase → lowercase
        }
    }

    printf("Toggled string: %s", str);
    
    return 0;
    }

DAY-46

//Remove all vowels from a string.

    #include <stdio.h>

    int main() {
        char str[200], result[200];
        int i = 0, j = 0;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    while (str[i] != '\0') {
        char ch = str[i];
        // Check if vowel
        if (!(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
              ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U')) {
            result[j] = ch;
            j++;
        }
        i++;
    }

    result[j] = '\0';

    printf("String after removing vowels: %s", result);

    return 0;
    }
    
//Find the first repeating lowercase alphabet in a string.

    #include <stdio.h>

    int main() {
        char str[100];
        int freq[26] = {0};

    printf("Enter a lowercase string: ");
    scanf("%[^\n]", str);

    // Count frequency
    for (int i = 0; str[i] != '\0'; i++) {
        if (str[i] >= 'a' && str[i] <= 'z') {
            freq[str[i] - 'a']++;
            if (freq[str[i] - 'a'] == 2) {
                printf("First repeating character: %c\n", str[i]);
                return 0;
            }
        }
    }

    printf("No repeating lowercase alphabet found.\n");
    return 0;
    }
DAY-47

//Check if two strings are anagrams of each other.

     #include <stdio.h>
     #include <string.h>

    int main() {
         char str1[100], str2[100];
         int freq1[26] = {0}, freq2[26] = {0};

    printf("Enter first string: ");
    scanf("%s", str1);

    printf("Enter second string: ");
    scanf("%s", str2);

    if (strlen(str1) != strlen(str2)) {
        printf("Not anagrams\n");
        return 0;
    }

    // Count frequency of each character in str1
    for (int i = 0; str1[i] != '\0'; i++) {
        freq1[str1[i] - 'a']++;
    }

    // Count frequency of each character in str2
    for (int i = 0; str2[i] != '\0'; i++) {
        freq2[str2[i] - 'a']++;
    }

    // Compare both frequency arrays
    for (int i = 0; i < 26; i++) {
        if (freq1[i] != freq2[i]) {
            printf("Not anagrams\n");
            return 0;
        }
    }

    printf("Anagrams\n");
    return 0;
    }
//Find the longest word in a sentence.

    #include <stdio.h>
    #include <string.h>

    int main() {
        char str[200];
        char longest[200];
        int maxLen = 0, currLen = 0;
        int i = 0, start = 0, longestStart = 0;

    printf("Enter a sentence: ");
    fgets(str, sizeof(str), stdin);

    // Loop through the string
    while (str[i] != '\0') {
        if (str[i] != ' ' && str[i] != '\n') {
            currLen++;
        } else {
            if (currLen > maxLen) {
                maxLen = currLen;
                longestStart = start;
            }
            currLen = 0;
            start = i + 1;
        }
        i++;
    }

    // Check last word
    if (currLen > maxLen) {
        maxLen = currLen;
        longestStart = start;
    }

    // Copy longest word
    for (i = 0; i < maxLen; i++) {
        longest[i] = str[longestStart + i];
    }
    longest[maxLen] = '\0';

    printf("Longest word: %s\n", longest);
    printf("Length: %d\n", maxLen);

    return 0;
    }
    
DAY-48

//Check if one string is a rotation of another.

    #include <stdio.h>
    #include <string.h>

    int main() {
        char str1[100], str2[100], temp[200];

    printf("Enter first string: ");
    gets(str1);

    printf("Enter second string: ");
    gets(str2);

    // If lengths differ, cannot be rotation
    if (strlen(str1) != strlen(str2)) {
        printf("Not a rotation.\n");
        return 0;
    }

    // Make temp = str1 + str1  (concatenate)
    strcpy(temp, str1);
    strcat(temp, str1);

    // If str2 is a substring of temp → rotation
    if (strstr(temp, str2) != NULL)
        printf("Rotation.\n");
    else
        printf("Not a rotation.\n");
    return 0;

 //Reverse each word in a sentence without changing the word order.

    #include <stdio.h>

    int main() {
        char str[200];
        int i = 0, start = 0;

    printf("Enter a sentence: ");
    fgets(str, sizeof(str), stdin);

    while (str[i] != '\0') {
        // When a word ends (space or end of string)
        if (str[i] == ' ' || str[i] == '\n' || str[i] == '\0') {
            int end = i - 1;

            // Reverse the word manually
            while (start < end) {
                char temp = str[start];
                str[start] = str[end];
                str[end] = temp;
                start++;
                end--;
            }
            start = i + 1;  // Move to next word's start
        }
        i++;
    }

    printf("Reversed words sentence:\n%s", str);

    return 0;
    }
    
 DAY-49

 //Print the initials of a name.
 
    #include <stdio.h>

     int main() {
         char str[100];

    printf("Enter your full name: ");
    fgets(str, sizeof(str), stdin);

    // Print the first initial
    if (str[0] != ' ') {
        printf("%c ", str[0]);
    }

    // Print initials after spaces
    for (int i = 1; str[i] != '\0'; i++) {
        if (str[i] == ' ' && str[i + 1] != ' ' && str[i + 1] != '\0') {
            printf("%c ", str[i + 1]);
        }
    }

    return 0;
    }
//Print initials of a name with the surname displayed in full.

    #include <stdio.h>

    int main() {
        char name[100];
        int i = 0;

    printf("Enter your full name: ");
    fgets(name, sizeof(name), stdin);

    // Print the first initial
    if (name[0] != ' ')
        printf("%c. ", name[0]);

    // Find and print the surname (last word)
    int lastStart = 0;
    for (i = 0; name[i] != '\0'; i++) {
        if (name[i] == ' ' && name[i+1] != ' ' && name[i+1] != '\0')
            lastStart = i + 1;  // start of last word
    }

    // Print the surname
    for (i = lastStart; name[i] != '\0' && name[i] != '\n'; i++) {
        printf("%c", name[i]);
    }

    return 0;
    }
    
DAY-50

//Change the date format from dd/04/yyyy to dd-Apr-yyyy.

    #include <stdio.h>

    int main() {
        char date[20];
        int day, year;

    printf("Enter date in dd/04/yyyy format: ");
    scanf("%s", date);

    sscanf(date, "%d/04/%d", &day, &year);

    printf("%02d-Apr-%d\n", day, year);

    return 0;
    }
//Print all sub-strings of a string.

    #include <stdio.h>

    int main() {
        char str[100];
        int i, j, k;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);

    // Remove newline if present
    for (i = 0; str[i] != '\0'; i++) {
        if (str[i] == '\n')
            str[i] = '\0';
    }

    // Print all substrings
    for (i = 0; str[i] != '\0'; i++) {
        for (j = i; str[j] != '\0'; j++) {
            for (k = i; k <= j; k++) {
                printf("%c", str[k]);
            }
            printf("\n");
        }
    }

    return 0;
    }
    
 DAY-51

 //Write a Program to take a sorted array(say nums[]) and an integer (say target) as inputs. The elements in the sorted array might be repeated. You need to print the first and last occurrence of the target and print the index of first and last occurrence. Print -1, -1 if the target is not present.

    #include <stdio.h>

    int main() {
        int n, target;
    
    printf("Enter size of array: ");
    scanf("%d", &n);
    
    int nums[n];
    
    printf("Enter %d sorted elements: \n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &nums[i]);
    }
    
    printf("Enter target: ");
    scanf("%d", &target);
    
    int first = -1, last = -1;
    
    // Find first and last occurrence
    for (int i = 0; i < n; i++) {
        if (nums[i] == target) {
            if (first == -1) {
                first = i;       // first occurrence
            }
            last = i;            // last occurrence keeps updating
        }
    }
    
    // Print results
    printf("First occurrence: %d\n", first);
    printf("Last occurrence: %d\n", last);

    return 0;
    }
    
DAY-52

//Write a Program to take a sorted array arr[] and an integer x as input, find the index (0-based) of the smallest element in arr[] that is greater than or equal to x and print it. This element is called the ceil of x. If such an element does not exist, print -1. Note: In case of multiple occurrences of ceil of x, return the index of the first occurrence.

    #include <stdio.h>

    int main() {
        int n, x;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d sorted elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter x: ");
    scanf("%d", &x);

    int low = 0, high = n - 1;
    int answer = -1;

    // Binary search for ceil of x
    while (low <= high) {
        int mid = (low + high) / 2;

        if (arr[mid] >= x) {
            answer = mid;       // possible ceil
            high = mid - 1;     // try to find earlier occurrence
        } else {
            low = mid + 1;
        }
    }

    printf("%d\n", answer);   // prints index or -1

    return 0;
    }
    
DAY-53

//Write a Program to take an array of integers as input, calculate the pivot index of this array. The pivot index is the index where the sum of all the numbers strictly to the left of the index is equal to the sum of all the numbers strictly to the index's right. If the index is on the left edge of the array, then the left sum is 0 because there are no elements to the left. This also applies to the right edge of the array. Print the leftmost pivot index. If no such index exists, print -1.

    #include <stdio.h>

    int main() {
       int n;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int totalSum = 0;
    for (int i = 0; i < n; i++) {
        totalSum += arr[i];
    }

    int leftSum = 0;

    for (int i = 0; i < n; i++) {
        int rightSum = totalSum - leftSum - arr[i];

        if (leftSum == rightSum) {
            printf("%d\n", i);
            return 0;   // print leftmost pivot index
        }

        leftSum += arr[i];
    }

    // If no pivot index found
    printf("-1\n");
    return 0;
    }
    
DAY-54

//Write a Program to take a positive integer n as input, and find the pivot integer x such that the sum of all elements between 1 and x inclusively equals the sum of all elements between x and n inclusively. Print the pivot integer x. If no such integer exists, print -1. Assume that it is guaranteed that there will be at most one pivot integer for the given input.

    #include <stdio.h>

    int main() {
        int n;
        printf("Enter n: ");
        scanf("%d", &n);

    // Total sum from 1 to n
    int total = n * (n + 1) / 2;

    // Try each x from 1 to n
    for (int x = 1; x <= n; x++) {
        long long leftSum = x * (x + 1) / 2;
        long long rightSum = total - (x - 1) * x / 2;

        if (leftSum == rightSum) {
            printf("%d\n", x);
            return 0;
        }
    }

    printf("-1\n");  // No pivot found
    return 0;
    }
    
DAY-55

//Write a program to take an integer array nums of size n, and print the majority element. The majority element is the element that appears strictly more than ⌊n / 2⌋ times. Print -1 if no such element exists. Note: Majority Element is not necessarily the element that is present most number of times.

    #include <stdio.h>

    int main() {
        int n;
        printf("Enter size of array: ");
        scanf("%d", &n);

    int nums[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &nums[i]);
    }

    // Boyer-Moore Voting Algorithm to find candidate
    int candidate = 0, count = 0;

    for (int i = 0; i < n; i++) {
        if (count == 0) {
            candidate = nums[i];
            count = 1;
        } else if (nums[i] == candidate) {
            count++;
        } else {
            count--;
        }
    }

    // Verify if the candidate is actually a majority element
    count = 0;
    for (int i = 0; i < n; i++) {
        if (nums[i] == candidate) {
            count++;
        }
    }

    if (count > n / 2)
        printf("%d\n", candidate);
    else
        printf("-1\n");

    return 0;
    }

DAY-56

//Write a program to take an array arr[] of integers as input, the task is to find the next greater element for each element of the array in order of their appearance in the array. Next greater element of an element in the array is the nearest element on the right which is greater than the current element. If there does not exist next greater of current element, then next greater element for current element is -1.

N.B:
- Print the output for each element in a comma separated fashion.
- Do not use Stack, use brute force approach (nested loop) to solve.

      #include <stdio.h>

      int main() {
          int n;
          printf("Enter size of array: ");
          scanf("%d", &n);

       int arr[n], nge[n], stack[n];
       int top = -1;

       printf("Enter %d elements:\n", n);
      for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
      }

      // Process from right to left
      for (int i = n - 1; i >= 0; i--) {

        // Pop all elements smaller or equal to arr[i]
        while (top != -1 && stack[top] <= arr[i]) {
            top--;
        }

        // If empty, no greater element
        nge[i] = (top == -1) ? -1 : stack[top];

        // Push current element
        stack[++top] = arr[i];
       }

       // Print result in comma-separated format
      for (int i = 0; i < n; i++) {
        printf("%d", nge[i]);
        if (i != n - 1)
            printf(", ");
       }

         return 0;
       }
    
DAY-57

//Write a program to take an array arr[] of integers as input, the task is to find the previous greater element for each element of the array in order of their appearance in the array. Previous greater element of an element in the array is the nearest element on the left which is greater than the current element. If there does not exist next greater of current element, then previous greater element for current element is -1.

N.B:
- Print the output for each element in a comma separated fashion.
- Do not use Stack, use brute force approach (nested loop) to solve.

      #include <stdio.h>

      int main() {
          int n;
          printf("Enter size of array: ");
           scanf("%d", &n);

          int arr[n], pge[n], stack[n];
          int top = -1;

           printf("Enter %d elements:\n", n);
           for (int i = 0; i < n; i++) {
              scanf("%d", &arr[i]);
          }

         // Process from left to right
         for (int i = 0; i < n; i++) {

        // Pop all elements <= current element
        while (top != -1 && stack[top] <= arr[i]) {
            top--;
        }

        // If stack empty → no previous greater
        if (top == -1)
            pge[i] = -1;
        else
            pge[i] = stack[top];

        // Push current element
        stack[++top] = arr[i];
        }

        // Print comma-separated output
       for (int i = 0; i < n; i++) {
        printf("%d", pge[i]);
        if (i != n - 1)
            printf(", ");
      }

      return 0;
      }
    
DAY-58

//Write a Program to take an integer array nums. Print an array answer such that answer[i] is equal to the product of all the elements of nums except nums[i]. The product of any prefix or suffix of nums is guaranteed to fit in a 32-bit integer.

    #include <stdio.h>

    int main() {
    int n;
    printf("Enter size of array: ");
    scanf("%d", &n);

    int nums[n], answer[n], prefix[n], suffix[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &nums[i]);
    }

    // Build prefix product array
    prefix[0] = 1;
    for (int i = 1; i < n; i++) {
        prefix[i] = prefix[i - 1] * nums[i - 1];
    }

    // Build suffix product array
    suffix[n - 1] = 1;
    for (int i = n - 2; i >= 0; i--) {
        suffix[i] = suffix[i + 1] * nums[i + 1];
    }

    // Build final answer
    for (int i = 0; i < n; i++) {
        answer[i] = prefix[i] * suffix[i];
    }

    // Print in comma-separated format
    for (int i = 0; i < n; i++) {
        printf("%d", answer[i]);
        if (i != n - 1) printf(", ");
    }

    return 0;
    }
    
DAY-59

//Write a program to take an integer array arr and an integer k as inputs. Print the maximum sum of all the subarrays of size k.

    #include <stdio.h>

    int main() {
        int n, k;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter k: ");
    scanf("%d", &k);

    // Edge case: if k > n, no subarray possible
    if (k > n) {
        printf("-1\n");
        return 0;
    }

    int currentSum = 0;

    // First window sum
    for (int i = 0; i < k; i++) {
        currentSum += arr[i];
    }

    int maxSum = currentSum;

    // Slide the window
    for (int i = k; i < n; i++) {
        currentSum = currentSum - arr[i - k] + arr[i];
        if (currentSum > maxSum)
            maxSum = currentSum;
    }

    printf("%d\n", maxSum);

    return 0;
    }
    
DAY-60

//Write a program to take an integer array arr and an integer k as inputs. The task is to find the maximum element in each subarray of size k moving from left to right. Print the maximum elements for each window separated by spaces as output.

    #include <stdio.h>

    int main() {
        int n, k;
         printf("Enter size of array: ");
         scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter k: ");
    scanf("%d", &k);

    if (k > n) {
        printf("-1\n");
        return 0;
    }

    int deque[n];  // stores indices
    int front = 0, back = -1;

    // Process first k elements (first window)
    for (int i = 0; i < k; i++) {
        while (front <= back && arr[deque[back]] <= arr[i])
            back--;
        deque[++back] = i;
    }

    // For the rest of windows
    for (int i = k; i < n; i++) {

        // Print max of previous window
        printf("%d ", arr[deque[front]]);

        // Remove elements that are out of this window
        while (front <= back && deque[front] <= i - k)
            front++;

        // Remove smaller elements as they are useless
        while (front <= back && arr[deque[back]] <= arr[i])
            back--;

        deque[++back] = i;
    }

    // Print max of last window
    printf("%d", arr[deque[front]]);

    return 0;
    }
    
DAY-61

//Write a program to take an integer array arr and an integer k as inputs. The task is to find the first negative integer in each subarray of size k moving from left to right. If no negative exists in a window, print "0" for that window. Print the results separated by spaces as output.

    #include <stdio.h>

    int main() {
        int n, k;
        printf("Enter size of array: ");
         scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter k: ");
    scanf("%d", &k);

    if (k > n) {
        printf("-1\n");
        return 0;
    }

    int negIndices[n];
    int front = 0, back = -1;

    // Process first window
    for (int i = 0; i < k; i++) {
        if (arr[i] < 0)
            negIndices[++back] = i;
    }

    // Slide through the array
    for (int i = k; i < n; i++) {

        // Print first negative of previous window
        if (front <= back)
            printf("%d ", arr[negIndices[front]]);
        else
            printf("0 ");

        // Remove elements that go out of the window
        while (front <= back && negIndices[front] <= i - k)
            front++;

        // Add the new index if negative
        if (arr[i] < 0)
            negIndices[++back] = i;
    }

    // Print result for the last window
    if (front <= back)
        printf("%d", arr[negIndices[front]]);
    else
        printf("0");

    return 0;
    }

DAY-62

//Write a program to take an integer array arr as input. The task is to find the maximum sum of any contiguous subarray using Kadane's algorithm. Print the maximum sum as output. If all elements are negative, print the largest (least negative) element.

    #include <stdio.h>

    int main() {
        int n;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    int maxEndingHere = arr[0];
    int maxSoFar = arr[0];

    for (int i = 1; i < n; i++) {
        // choose max: extend previous sum OR start new from arr[i]
        if (maxEndingHere + arr[i] > arr[i])
            maxEndingHere = maxEndingHere + arr[i];
        else
            maxEndingHere = arr[i];

        // update global maximum
        if (maxEndingHere > maxSoFar)
            maxSoFar = maxEndingHere;
    }

    printf("%d\n", maxSoFar);

    return 0;
    }
    
DAY-63

//Write a program to take an integer array arr and an integer k as inputs. The task is to find the kth smallest element in the array. Print the kth smallest element as output.

    #include <stdio.h>

    // Simple swap function
    void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
    }

    // Bubble sort (simple for beginners)
    void sortArray(int arr[], int n) {
    for (int i = 0; i < n - 1; i++) {
        for (int j = 0; j < n - 1 - i; j++) {
            if (arr[j] > arr[j + 1]) {
                swap(&arr[j], &arr[j + 1]);
            }
        }
    }
    }

    int main() {
        int n, k;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int arr[n];

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter k: ");
    scanf("%d", &k);

    if (k < 1 || k > n) {
        printf("-1\n");
        return 0;
    }

    sortArray(arr, n);

    printf("%d\n", arr[k - 1]);  // k-th smallest after sorting

    return 0;
    }
    
DAY-64

//Write a program to take a string s as input. The task is to find the length of the longest substring without repeating characters. Print the length as output.

    #include <stdio.h>
    #include <string.h>

    int main() {
        char s[1000];
    
    printf("Enter the string: ");
    scanf("%[^\n]%*c", s);  // read full line including spaces

    int freq[256] = {0};  // frequency of characters
    int left = 0, maxLen = 0;

    for (int right = 0; s[right] != '\0'; right++) {
        char c = s[right];
        freq[(unsigned char)c]++;

        // If character repeats, shrink window
        while (freq[(unsigned char)c] > 1) {
            freq[(unsigned char)s[left]]--;
            left++;
        }

        // Update maximum length
        int windowLen = right - left + 1;
        if (windowLen > maxLen)
            maxLen = windowLen;
    }

    printf("%d\n", maxLen);

    return 0;
    }
    
DAY-65

//Write a program to take two strings s and t as inputs (assume all characters are lowercase). The task is to determine if s and t are valid anagrams, meaning they contain the same characters with the same frequencies. Print "Anagram" if they are, otherwise "Not Anagram".

    #include <stdio.h>
    #include <string.h>

    int main() {
         char s[1000], t[1000];

    printf("Enter string s: ");
    scanf("%s", s);

    printf("Enter string t: ");
    scanf("%s", t);

    // If lengths differ, they cannot be anagrams
    if (strlen(s) != strlen(t)) {
        printf("Not Anagram\n");
        return 0;
    }

    int freq[26] = {0};

    // Count characters of s and t
    for (int i = 0; s[i] != '\0'; i++) {
        freq[s[i] - 'a']++;
        freq[t[i] - 'a']--;
    }

    // Check if all frequencies become zero
    for (int i = 0; i < 26; i++) {
        if (freq[i] != 0) {
            printf("Not Anagram\n");
            return 0;
        }
    }

    printf("Anagram\n");
    return 0;
    }
    
DAY-66

//Write a program to take an integer array nums which contains only positive integers, and an integer target as inputs. The goal is to find two distinct indices i and j in the array such that nums[i] + nums[j] equals the target. Assume exactly one solution exists and return the indices in any order. Print the two indices separated by a space as output. If no solution exists, print "-1 -1".

    #include <stdio.h>

    int main() {
        int n, target;

    printf("Enter size of array: ");
    scanf("%d", &n);

    int nums[n];

    printf("Enter %d positive integers:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &nums[i]);
    }

    printf("Enter target: ");
    scanf("%d", &target);

    // Brute-force O(n^2)
    for (int i = 0; i < n; i++) {
        for (int j = i + 1; j < n; j++) {
            if (nums[i] + nums[j] == target) {
                printf("%d %d\n", i, j);
                return 0; // exactly one solution exists
            }
        }
    }

    // If no solution found
    printf("-1 -1\n");
    return 0;
    }
    
DAY-67

//Write a program to take two sorted arrays of size m and n as input. Merge both the arrays such that the merged array is also sorted. Print the merged array.

    #include <stdio.h>

    int main() {
        int m, n;

    printf("Enter size of first array: ");
    scanf("%d", &m);
    int arr1[m];

    printf("Enter %d sorted elements:\n", m);
    for (int i = 0; i < m; i++) {
        scanf("%d", &arr1[i]);
    }

    printf("Enter size of second array: ");
    scanf("%d", &n);
    int arr2[n];

    printf("Enter %d sorted elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr2[i]);
    }

    int merged[m + n];
    int i = 0, j = 0, k = 0;

    // Merge using two pointers
    while (i < m && j < n) {
        if (arr1[i] <= arr2[j]) {
            merged[k++] = arr1[i++];
        } else {
            merged[k++] = arr2[j++];
        }
    }

    // Copy remaining elements
    while (i < m) {
        merged[k++] = arr1[i++];
    }

    while (j < n) {
        merged[k++] = arr2[j++];
    }

    // Print merged array
    for (int x = 0; x < m + n; x++) {
        printf("%d", merged[x]);
        if (x != m + n - 1) printf(" ");
    }

    return 0;
    }
DAY-68

//Write a program to take an input array of size n. The array should contain all the integers between 0 to n except for one. Print that missing number

    #include <stdio.h>

    int main() {
        int n;
        printf("Enter n: ");
        scanf("%d", &n);

    int arr[n];
    int sum = 0;

    printf("Enter %d elements (0 to %d with one missing):\n", n, n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        sum += arr[i];
    }

    // Expected sum of numbers from 0 to n
    int total = n * (n + 1) / 2;

    int missing = total - sum;

    printf("%d\n", missing);

    return 0;
    }

DAY-69

//Write a program to take an integer array as input. Only one element will be repeated. Print the repeated element. Try to find the result in one single iteration.

    #include <stdio.h>

    int main() {
         int n;
         printf("Enter size of array: ");
        scanf("%d", &n);

    int arr[n];
    printf("Enter %d integers (one will be repeated):\n", n);

    // XOR of all array elements
    int xorAll = 0;
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        xorAll ^= arr[i];       // XOR the element
    }

    // XOR numbers from 0 to n-2
    for (int i = 0; i <= n - 2; i++) {
        xorAll ^= i;
    }

    // Remaining value is the repeated number
    printf("%d\n", xorAll);

    return 0;
    }

DAY-70

//Write a program to take a string input. Change it to sentence case.

     #include <stdio.h>
    #include <ctype.h>

    int main() {
       char s[1000];

    printf("Enter a string: ");
    scanf("%[^\n]%*c", s);   // read full line including spaces

    // Convert first character to uppercase (if alphabet)
    if (s[0] != '\0') {
        s[0] = toupper(s[0]);
    }

    // Convert all other characters to lowercase
    for (int i = 1; s[i] != '\0'; i++) {
        s[i] = tolower(s[i]);
    }

    printf("%s\n", s);

    return 0;
    }

DAY-71

//Write a C program that creates a text file named info.txt in write mode. The program should take the user’s name and age as input, and write them to the file using fprintf(). After writing, display a message confirming that the data was successfully saved.

    #include <stdio.h>

    int main() {
        FILE *fp;
        char name[100];
        int age;

    // Open file in write mode
    fp = fopen("info.txt", "w");

    if (fp == NULL) {
        printf("Error opening file!\n");
        return 1;
    }

    // Take user input
    printf("Enter your name: ");
    scanf("%[^\n]", name);

    printf("Enter your age: ");
    scanf("%d", &age);

    // Write to file
    fprintf(fp, "Name: %s\nAge: %d\n", name, age);

    // Close file
    fclose(fp);

    printf("Data successfully saved to info.txt\n");

    return 0;
    }

DAY-72

//Write a C program that opens an existing file (e.g., info.txt) and reads its contents using fgets(). The program should print all the lines to the console until EOF (end of file) is reached.

    #include <stdio.h>

    int main() {
         FILE *fp;
         char line[200];

    // Open file in read mode
    fp = fopen("info.txt", "r");

    if (fp == NULL) {
        printf("Error: Could not open file.\n");
        return 1;
    }

    printf("Contents of info.txt:\n\n");

    // Read lines until EOF
    while (fgets(line, sizeof(line), fp) != NULL) {
        printf("%s", line);
    }

    // Close the file
    fclose(fp);

    return 0;
     }

DAY-73

//Read a text file and count the total number of characters, words, and lines. A word is defined as a sequence of non-space characters separated by spaces or newlines.

    #include <stdio.h>
    #include <ctype.h>

     int main() {
         FILE *fp;
         char filename[100];
         char c;

    int characters = 0, words = 0, lines = 0;
    int inWord = 0; // flag to track word boundaries

    printf("Enter filename: ");
    scanf("%s", filename);

    fp = fopen(filename, "r");

    if (fp == NULL) {
        printf("Error: Could not open file.\n");
        return 1;
    }

    while ((c = fgetc(fp)) != EOF) {
        characters++;

        // Count lines
        if (c == '\n')
            lines++;

        // Detect word start
        if (!isspace(c) && inWord == 0) {
            inWord = 1;
            words++;
        }
        // Detect end of a word
        else if (isspace(c)) {
            inWord = 0;
        }
    }

    // If file doesn't end with newline, lines still fine
    // No need to adjust

    fclose(fp);

    printf("Characters: %d\n", characters);
    printf("Words: %d\n", words);
    printf("Lines: %d\n", lines);

    return 0;
    }

DAY-74

//Take two filenames from the user – a source file and a destination file. Copy all the content from the source file to the destination file using fgetc() and fputc().

    #include <stdio.h>

    int main() {
        char src[100], dest[100];
        FILE *fpSrc, *fpDest;
        int ch;

    // Take filenames from user
    printf("Enter source file name: ");
    scanf("%s", src);

    printf("Enter destination file name: ");
    scanf("%s", dest);

    // Open source in read mode
    fpSrc = fopen(src, "r");
    if (fpSrc == NULL) {
        printf("Error: Could not open source file.\n");
        return 1;
    }

    // Open destination in write mode
    fpDest = fopen(dest, "w");
    if (fpDest == NULL) {
        printf("Error: Could not create destination file.\n");
        fclose(fpSrc);
        return 1;
    }

    // Copy character by character
    while ((ch = fgetc(fpSrc)) != EOF) {
        fputc(ch, fpDest);
    }

    // Close both files
    fclose(fpSrc);
    fclose(fpDest);

    printf("File copied successfully from %s to %s\n", src, dest);

    return 0;
    }

DAY-75

//Open an existing file in append mode and allow the user to enter a new line of text. Append the text at the end without overwriting existing content.

    #include <stdio.h>

    int main() {
        char filename[100];
         char line[500];
        FILE *fp;

    // Take file name
    printf("Enter file name: ");
    scanf("%s", filename);
    getchar(); // clear leftover newline from input buffer

    // Open file in append mode
    fp = fopen(filename, "a");
    if (fp == NULL) {
        printf("Error: Could not open file.\n");
        return 1;
    }

    // Take new line of text from user
    printf("Enter text to append: ");
    fgets(line, sizeof(line), stdin);

    // Append the text
    fputs(line, fp);

    fclose(fp);

    printf("Text appended successfully.\n");

    return 0;
    }
    
DAY-76

//Ask the user for a filename. Check if it exists by trying to open it in read mode. If the file pointer is NULL, print an error message; otherwise, read and display its content.

    #include <stdio.h>

    int main() {
        char filename[100];
    FILE *fp;
    char ch;

    printf("Enter filename: ");
    scanf("%s", filename);

    // Try to open file in read mode
    fp = fopen(filename, "r");

    if (fp == NULL) {
        printf("Error: File does not exist or cannot be opened.\n");
        return 1;
    }

    printf("\n--- File Content ---\n\n");

    // Read and print character by character
    while ((ch = fgetc(fp)) != EOF) {
        putchar(ch);
    }

    fclose(fp);

    return 0;
    }

DAY-77

//Write a program that reads text from input.txt, converts all lowercase letters to uppercase, and writes the result to output.txt.

    #include <stdio.h>
    #include <ctype.h>

    int main() {
        FILE *inFile, *outFile;
        int ch;

    // Open input file in read mode
    inFile = fopen("input.txt", "r");
    if (inFile == NULL) {
        printf("Error: Could not open input.txt\n");
        return 1;
    }

    // Open output file in write mode
    outFile = fopen("output.txt", "w");
    if (outFile == NULL) {
        printf("Error: Could not create output.txt\n");
        fclose(inFile);
        return 1;
    }

    // Read each character, convert to uppercase, write to output.txt
    while ((ch = fgetc(inFile)) != EOF) {
        ch = toupper(ch);    // convert lowercase to uppercase
        fputc(ch, outFile);
    }

    fclose(inFile);
    fclose(outFile);

    printf("Conversion complete! Check output.txt\n");

    return 0;
    }

DAY-78

//Read a text file and count how many vowels and consonants are in the file. Ignore digits and special characters.

    #include <stdio.h>
    #include <ctype.h>

     int main() {
         FILE *fp;
         char filename[100];
         int ch;
         int vowels = 0, consonants = 0;

    printf("Enter filename: ");
    scanf("%s", filename);

    fp = fopen(filename, "r");

    if (fp == NULL) {
        printf("Error: Could not open file.\n");
        return 1;
    }

    while ((ch = fgetc(fp)) != EOF) {
        ch = tolower(ch);  // make counting easier

        // Check if alphabet
        if (ch >= 'a' && ch <= 'z') {
            // Check vowel
            if (ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u')
                vowels++;
            else
                consonants++;
        }
    }

    fclose(fp);

    printf("Vowels: %d\n", vowels);
    printf("Consonants: %d\n", consonants);

    return 0;
    }

DAY-79

//A file numbers.txt contains a list of integers separated by spaces. Read all integers, compute their sum and average, and print both.

    #include <stdio.h>

    int main() {
        FILE *fp;
        int num;
        int sum = 0, count = 0;

    fp = fopen("numbers.txt", "r");

    if (fp == NULL) {
        printf("Error: Could not open numbers.txt\n");
        return 1;
    }

    // Read integers until EOF
    while (fscanf(fp, "%d", &num) == 1) {
        sum += num;
        count++;
    }

    fclose(fp);

    if (count == 0) {
        printf("No numbers found in the file.\n");
        return 0;
    }

    float average = (float)sum / count;

    printf("Sum = %d\n", sum);
    printf("Average = %.2f\n", average);

    return 0;
    }

DAY-80

//Store multiple student records (name, roll number, marks) into a file using fprintf(). Then read them using fscanf() and display each record.

    #include <stdio.h>

    struct Student {
        char name[50];
        int roll;
        float marks;
    };

    int main() {
    FILE *fp;
    int n;

    printf("Enter number of students: ");
    scanf("%d", &n);

    struct Student s[n];

    // Take student details
    printf("\nEnter student details:\n");
    for (int i = 0; i < n; i++) {
        printf("\nStudent %d:\n", i + 1);

        printf("Name: ");
        scanf("%s", s[i].name);

        printf("Roll Number: ");
        scanf("%d", &s[i].roll);

        printf("Marks: ");
        scanf("%f", &s[i].marks);
    }

    // Write to file
    fp = fopen("students.txt", "w");
    if (fp == NULL) {
        printf("Error opening file.\n");
        return 1;
    }

    for (int i = 0; i < n; i++) {
        fprintf(fp, "%s %d %.2f\n", s[i].name, s[i].roll, s[i].marks);
    }

    fclose(fp);

    printf("\nData successfully written to students.txt\n");

    // Read from file
    fp = fopen("students.txt", "r");
    if (fp == NULL) {
        printf("Error reading file.\n");
        return 1;
    }

    printf("\n--- Student Records from File ---\n");

    struct Student temp;
    while (fscanf(fp, "%s %d %f", temp.name, &temp.roll, &temp.marks) == 3) {
        printf("Name: %s, Roll: %d, Marks: %.2f\n",
               temp.name, temp.roll, temp.marks);
    }

    fclose(fp);

    return 0;
    }

DAY-81

//Create an enumeration for days (SUNDAY to SATURDAY) and print each day with its integer value.

    #include <stdio.h>

    int main(void) {
        // Enumeration: by default SUNDAY = 0, MONDAY = 1, ..., SATURDAY = 6
        enum Day { SUNDAY, MONDAY, TUESDAY, WEDNESDAY, THURSDAY, FRIDAY, SATURDAY };

    const char *dayNames[] = {
        "SUNDAY", "MONDAY", "TUESDAY", "WEDNESDAY", "THURSDAY", "FRIDAY", "SATURDAY"
    };

    printf("Day name\tInteger value\n");
    printf("-------------------------------\n");

    for (int d = SUNDAY; d <= SATURDAY; d++) {
        printf("%-9s\t% d\n", dayNames[d], d);
    }

    return 0;
     }

DAY-82

//Define an enum for traffic lights (RED, YELLOW, GREEN) and print 'Stop', 'Wait', or 'Go' based on its value.

    #include <stdio.h>

    int main() {
       // Define enum
       enum TrafficLight { RED, YELLOW, GREEN };

    // Example: set current light here
    enum TrafficLight light;

    printf("Enter traffic light value (0=RED, 1=YELLOW, 2=GREEN): ");
    scanf("%d", &light);

    switch (light) {
        case RED:
            printf("Stop\n");
            break;
        case YELLOW:
            printf("Wait\n");
            break;
        case GREEN:
            printf("Go\n");
            break;
        default:
            printf("Invalid input\n");
            break;
    }

    return 0;
    }

DAY-83

//Create an enum for months and print how many days each month has.

    #include <stdio.h>

    int main() {
        // Enum for months
        enum Month {
        JANUARY, FEBRUARY, MARCH, APRIL, MAY, JUNE,
        JULY, AUGUST, SEPTEMBER, OCTOBER, NOVEMBER, DECEMBER
    };

    const char *monthNames[] = {
        "January", "February", "March", "April", "May", "June",
        "July", "August", "September", "October", "November", "December"
    };

    int days[] = {
        31, 28, 31, 30, 31, 30,
        31, 31, 30, 31, 30, 31
    };

    // Print all months with days
    for (int m = JANUARY; m <= DECEMBER; m++) {
        printf("%-10s : %d days\n", monthNames[m], days[m]);
    }

    return 0;
    }

DAY-84

//Define an enum with SUCCESS, FAILURE, and TIMEOUT, and print messages accordingly.

    #include <stdio.h>

    int main() {
       // Define enum
       enum Status { SUCCESS, FAILURE, TIMEOUT };

    enum Status status;

    // Ask user to enter a status code
    printf("Enter status (0=SUCCESS, 1=FAILURE, 2=TIMEOUT): ");
    scanf("%d", &status);

    // Print message based on status
    switch (status) {
        case SUCCESS:
            printf("Operation Successful\n");
            break;
        case FAILURE:
            printf("Operation Failed\n");
            break;
        case TIMEOUT:
            printf("Operation Timed Out\n");
            break;
        default:
            printf("Invalid Status Code\n");
            break;
    }

    return 0;
    }

DAY-85

//Assign explicit values starting from 10 and print them.

    #include <stdio.h>

    int main() {
        // Enum with explicit values
        enum Status {
        SUCCESS = 10,
        FAILURE = 11,
        TIMEOUT = 12
    };

    printf("SUCCESS = %d\n", SUCCESS);
    printf("FAILURE = %d\n", FAILURE);
    printf("TIMEOUT = %d\n", TIMEOUT);

    return 0;
    }

DAY-86

//Use enum to represent menu choices (ADD, SUBTRACT, MULTIPLY) and perform operations using switch.

    #include <stdio.h>

    int main() {
        // Define enum for menu choices
        enum Menu { ADD = 1, SUBTRACT, MULTIPLY };

    int choice;
    float a, b;

    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    printf("\nMenu:\n");
    printf("1. ADD\n");
    printf("2. SUBTRACT\n");
    printf("3. MULTIPLY\n");

    printf("Enter your choice (1-3): ");
    scanf("%d", &choice);

    switch (choice) {
        case ADD:
            printf("Result = %.2f\n", a + b);
            break;

        case SUBTRACT:
            printf("Result = %.2f\n", a - b);
            break;

        case MULTIPLY:
            printf("Result = %.2f\n", a * b);
            break;

        default:
            printf("Invalid choice.\n");
            break;
    }

    return 0;
    }

DAY-87

//Create an enum for user roles (ADMIN, USER, GUEST) and display messages based on role.

    #include <stdio.h>

    int main() {
       // Define enum for roles
        enum Role { ADMIN = 1, USER, GUEST };

    int role;

    printf("Select Role:\n");
    printf("1. ADMIN\n");
    printf("2. USER\n");
    printf("3. GUEST\n");

    printf("Enter choice (1-3): ");
    scanf("%d", &role);

    switch (role) {
        case ADMIN:
            printf("Welcome, Admin! You have full access.\n");
            break;

        case USER:
            printf("Hello User! You have limited access.\n");
            break;

        case GUEST:
            printf("Welcome Guest! You have view-only access.\n");
            break;

        default:
            printf("Invalid role selected.\n");
            break;
    }

    return 0;
    }

DAY-88

//Print all enum names and integer values using a loop.

    #include <stdio.h>

    int main() {
        // Define enum
        enum Role { ADMIN, USER, GUEST, SUPERADMIN };

    // Matching names for printing
    const char *roleNames[] = {
        "ADMIN", "USER", "GUEST", "SUPERADMIN"
    };

    // Print all enum values
    printf("Enum Name      Value\n");
    printf("-----------------------\n");

    for (int i = ADMIN; i <= SUPERADMIN; i++) {
        printf("%-12s %d\n", roleNames[i], i);
    }

    return 0;
    }

DAY-89

//Show that enums store integers by printing assigned values.

    #include <stdio.h>

    int main() {
    // Enum with explicit and implicit integer values
    enum Example {
        A = 5,   // assigned 5
        B,       // becomes 6
        C = 10,  // assigned 10
        D        // becomes 11
    };

    printf("A = %d\n", A);
    printf("B = %d\n", B);
    printf("C = %d\n", C);
    printf("D = %d\n", D);

    return 0;
    }

DAY-90

//Define a struct with enum Gender and print person's gender.

    #include <stdio.h>

    int main() {
       // Define enum for gender
       enum Gender { MALE = 1, FEMALE, OTHER };

    // Define struct containing the enum
    struct Person {
        char name[50];
        enum Gender gender;
    };

    struct Person p;

    // Take user input
    printf("Enter name: ");
    scanf("%s", p.name);

    printf("Select Gender (1=MALE, 2=FEMALE, 3=OTHER): ");
    scanf("%d", &p.gender);

    // Print Person Information
    printf("\nName: %s\n", p.name);

    switch (p.gender) {
        case MALE:
            printf("Gender: Male\n");
            break;
        case FEMALE:
            printf("Gender: Female\n");
            break;
        case OTHER:
            printf("Gender: Other\n");
            break;
        default:
            printf("Invalid Gender\n");
    }

    return 0;
    }

DAY-91

//Define a structure Student with name, roll_no, and marks, then read and print one student's data.

    #include <stdio.h>

    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    int main() {
    struct Student s;

    // Read student data
    printf("Enter student name: ");
    scanf("%s", s.name);

    printf("Enter roll number: ");
    scanf("%d", &s.roll_no);

    printf("Enter marks: ");
    scanf("%f", &s.marks);

    // Print student data
    printf("\n--- Student Details ---\n");
    printf("Name: %s\n", s.name);
    printf("Roll No: %d\n", s.roll_no);
    printf("Marks: %.2f\n", s.marks);

    return 0;
    }

DAY-92

//Store details of 5 students in an array of structures and print all.

     #include <stdio.h>

    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    int main() {
    struct Student s[5];

    // Input details of 5 students
    printf("Enter details of 5 students:\n");

    for (int i = 0; i < 5; i++) {
        printf("\nStudent %d:\n", i + 1);

        printf("Name: ");
        scanf("%s", s[i].name);

        printf("Roll No: ");
        scanf("%d", &s[i].roll_no);

        printf("Marks: ");
        scanf("%f", &s[i].marks);
    }

    // Output all student details
    printf("\n--- Student Details ---\n");

    for (int i = 0; i < 5; i++) {
        printf("\nStudent %d:\n", i + 1);
        printf("Name: %s\n", s[i].name);
        printf("Roll No: %d\n", s[i].roll_no);
        printf("Marks: %.2f\n", s[i].marks);
    }

    return 0;
    }

DAY-93

//Find and print the student with the highest marks.

    #include <stdio.h>

    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    int main() {
    struct Student s[5];
    int i, topIndex = 0;

    // Input 5 students
    printf("Enter details of 5 students:\n");

    for (i = 0; i < 5; i++) {
        printf("\nStudent %d:\n", i + 1);

        printf("Name: ");
        scanf("%s", s[i].name);

        printf("Roll No: ");
        scanf("%d", &s[i].roll_no);

        printf("Marks: ");
        scanf("%f", &s[i].marks);
    }

    // Find index of student with highest marks
    for (i = 1; i < 5; i++) {
        if (s[i].marks > s[topIndex].marks) {
            topIndex = i;
        }
    }

    // Print the topper
    printf("\n--- Student With Highest Marks ---\n");
    printf("Name: %s\n", s[topIndex].name);
    printf("Roll No: %d\n", s[topIndex].roll_no);
    printf("Marks: %.2f\n", s[topIndex].marks);

    return 0;
    }

DAY-94

//Write a function that accepts a structure as parameter and prints its members.

    #include <stdio.h>

    // Define structure
    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    // Function that accepts a structure and prints it
    void printStudent(struct Student s) {
    printf("\n--- Student Details ---\n");
    printf("Name: %s\n", s.name);
    printf("Roll No: %d\n", s.roll_no);
    printf("Marks: %.2f\n", s.marks);
    }

       struct Student st;

    // Read student details
    printf("Enter name: ");
    scanf("%s", st.name);

    printf("Enter roll number: ");
    scanf("%d", &st.roll_no);

    printf("Enter marks: ");
    scanf("%f", &st.marks);

    // Pass structure to function
    printStudent(st);

    return 0;
    }

DAY-95

//Return a structure containing top student's details from a function.

    #include <stdio.h>

    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    // Function that returns the student with highest marks
    struct Student getTopStudent(struct Student s[], int n) {
    int topIndex = 0;

    for (int i = 1; i < n; i++) {
        if (s[i].marks > s[topIndex].marks) {
            topIndex = i;
        }
    }

    return s[topIndex];  // return structure
    }

    int main() {
    int n;

    printf("Enter number of students: ");
    scanf("%d", &n);

    struct Student s[n];

    // Input
    for (int i = 0; i < n; i++) {
        printf("\nStudent %d:\n", i + 1);

        printf("Name: ");
        scanf("%s", s[i].name);

        printf("Roll No: ");
        scanf("%d", &s[i].roll_no);

        printf("Marks: ");
        scanf("%f", &s[i].marks);
    }

    // Get top student
    struct Student top = getTopStudent(s, n);

    // Output
    printf("\n--- Top Student ---\n");
    printf("Name : %s\n", top.name);
    printf("Roll No : %d\n", top.roll_no);
    printf("Marks : %.2f\n", top.marks);

    return 0;
    }

DAY-96

//Create Employee structure with nested Date structure for joining date and print details.

    #include <stdio.h>

    // Nested structure for Date
    struct Date {
    int day;
    int month;
    int year;
    };

    // Employee structure containing Date
    struct Employee {
    char name[50];
    int id;
    float salary;
    struct Date joiningDate;
    };

    int main() {
    struct Employee emp;

    // Input employee details
    printf("Enter Employee Name: ");
    scanf("%s", emp.name);

    printf("Enter Employee ID: ");
    scanf("%d", &emp.id);

    printf("Enter Salary: ");
    scanf("%f", &emp.salary);

    printf("Enter Joining Date (dd mm yyyy): ");
    scanf("%d %d %d", &emp.joiningDate.day,
                     &emp.joiningDate.month,
                     &emp.joiningDate.year);

    // Output employee details
    printf("\n--- Employee Details ---\n");
    printf("Name         : %s\n", emp.name);
    printf("ID           : %d\n", emp.id);
    printf("Salary       : %.2f\n", emp.salary);
    printf("Joining Date : %02d-%02d-%04d\n",
            emp.joiningDate.day,
            emp.joiningDate.month,
            emp.joiningDate.year);

    return 0;
    }

DAY-97

//Store employee data in a binary file using fwrite() and read using fread().

     #include <stdio.h>

    struct Employee {
    char name[50];
    int id;
    float salary;
     };

    int main() {
    FILE *fp;
    int n;

    printf("Enter number of employees: ");
    scanf("%d", &n);

    struct Employee e[n];

    // Input employee data
    for (int i = 0; i < n; i++) {
        printf("\nEmployee %d:\n", i + 1);

        printf("Name: ");
        scanf("%s", e[i].name);

        printf("ID: ");
        scanf("%d", &e[i].id);

        printf("Salary: ");
        scanf("%f", &e[i].salary);
    }

    // Write to binary file
    fp = fopen("employees.bin", "wb");
    if (fp == NULL) {
        printf("Error opening file for writing.\n");
        return 1;
    }

    fwrite(e, sizeof(struct Employee), n, fp);
    fclose(fp);

    printf("\nData successfully written to employees.bin\n");

    // Read from binary file
    fp = fopen("employees.bin", "rb");
    if (fp == NULL) {
        printf("Error opening file for reading.\n");
        return 1;
    }

    struct Employee temp;

    printf("\n--- Employee Records from File ---\n");

    while (fread(&temp, sizeof(struct Employee), 1, fp) == 1) {
        printf("\nName   : %s\n", temp.name);
        printf("ID     : %d\n", temp.id);
        printf("Salary : %.2f\n", temp.salary);
    }

    fclose(fp);

    return 0;
    }
    
DAY-98
    
//Take two structs as input and check if they are identical

    #include <stdio.h>

    // Manual string compare function
    int myStrCmp(char a[], char b[]) {
    int i = 0;
    while (a[i] != '\0' && b[i] != '\0') {
        if (a[i] != b[i])
            return 0;   // not equal
        i++;
    }
    // If both ended at same time → identical
    return (a[i] == '\0' && b[i] == '\0');
    }

    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    int main() {
    struct Student s1, s2;

    // Input for first student
    printf("Enter details of Student 1:\n");
    printf("Name: ");
    scanf("%s", s1.name);
    printf("Roll No: ");
    scanf("%d", &s1.roll_no);
    printf("Marks: ");
    scanf("%f", &s1.marks);

    // Input for second student
    printf("\nEnter details of Student 2:\n");
    printf("Name: ");
    scanf("%s", s2.name);
    printf("Roll No: ");
    scanf("%d", &s2.roll_no);
    printf("Marks: ");
    scanf("%f", &s2.marks);

    // Compare structures manually
    if (myStrCmp(s1.name, s2.name) &&
        s1.roll_no == s2.roll_no &&
        s1.marks == s2.marks) 
    {
        printf("\nThe structures are IDENTICAL.\n");
    } 
    else {
        printf("\nThe structures are NOT identical.\n");
    }

    return 0;
    }

DAY-99

//Use malloc() to allocate structure memory dynamically and print details.

    #include <stdio.h>
    #include <stdlib.h>

    struct Student {
    char name[50];
    int roll_no;
    float marks;
    };

    int main() {
    // Allocate structure dynamically
    struct Student *s = (struct Student *)malloc(sizeof(struct Student));

    if (s == NULL) {
        printf("Memory allocation failed!\n");
        return 1;
    }

    // Input details
    printf("Enter student name: ");
    scanf("%s", s->name);

    printf("Enter roll number: ");
    scanf("%d", &s->roll_no);

    printf("Enter marks: ");
    scanf("%f", &s->marks);

    // Output details
    printf("\n--- Student Details ---\n");
    printf("Name: %s\n", s->name);
    printf("Roll No: %d\n", s->roll_no);
    printf("Marks: %.2f\n", s->marks);

    // Free allocated memory
    free(s);

    return 0;
    }
