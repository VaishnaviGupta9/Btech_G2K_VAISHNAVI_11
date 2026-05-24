# Btech_G2K_VAISHNAVI_11
C Program
WAP to find sum of 5 numbers and average of it.
#include <stdio.h>

int main() {
    int n1, n2, n3, n4, n5;
    int sum;
    float average;

    printf("Enter 5 numbers:\n");

    scanf("%d%d%d%d%d", &n1, &n2, &n3, &n4, &n5);

    sum = n1 + n2 + n3 + n4 + n5;

    average = sum / 5.0;

    printf("Sum = %d\n", sum);
    printf("Average = %.2f\n", average);

    return 0;
}

2- WAP to find simple and compound interest.
#include <stdio.h>

int main() {
    float p, r, t, si;

    printf("Enter Principal Amount: ");
    scanf("%f", &p);

    printf("Enter Rate of Interest: ");
    scanf("%f", &r);

    printf("Enter Time: ");
    scanf("%f", &t);

    si = (p * r * t) / 100;

    printf("Simple Interest = %.2f", si);

    return 0;
}
3-WAP to find area and circumference of circle.
#include <stdio.h>

int main() {
    float radius, area, circumference;

    printf("Enter radius of circle: ");
    scanf("%f", &radius);

    area = 3.14 * radius * radius;
    circumference = 2 * 3.14 * radius;

    printf("Area of circle = %.2f\n", area);
    printf("Circumference of circle = %.2f", circumference);

    return 0;
}
4-WAP to convert celsius to frahernite.
#include <stdio.h>

int main() {
    float fahrenheit, celsius;

    printf("Enter temperature in Fahrenheit: ");
    scanf("%f", &fahrenheit);

    celsius = (fahrenheit - 32) * 5 / 9;

    printf("Temperature in Celsius = %.2f", celsius);

    return 0;
}
5-WAP to swap two variables using third variable.
#include <stdio.h>

int main() {
    int a, b, temp;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    temp = a;
    a = b;
    b = temp;

    printf("After swapping:\n");
    printf("a = %d\n", a);
    printf("b = %d", b);

    return 0;
}
6-WAP to check the number is even or add.
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if(num % 2 == 0)
        printf("Number is Even");
    else
        printf("Number is Odd");

    return 0;
}
7-WAP to find the factorial of the given number.
#include <stdio.h>

int main() {
    int num, i;
    long long factorial = 1;

    printf("Enter a number: ");
    scanf("%d", &num);

    for(i = 1; i <= num; i++) {
        factorial = factorial * i;
    }

    printf("Factorial = %lld", factorial);

    return 0;
}
8- WAP to find the entered year is leap or not #include <stdio.h>

int main() {
    int year;

    printf("Enter a year: ");
    scanf("%d", &year);

    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0))
        printf("%d is a Leap Year", year);
    else
        printf("%d is not a Leap Year", year);

    return 0;
}
9-WAP to find the greatest of 3 number.
#include <stdio.h>

int main() {
    int a, b, c;

    printf("Enter three numbers: ");
    scanf("%d %d %d", &a, &b, &c);

    if(a >= b && a >= c)
        printf("%d is the greatest", a);

    else if(b >= a && b >= c)
        printf("%d is the greatest", b);

    else
        printf("%d is the greatest", c);

    return 0;
}
10- WAP that accepts marks of 5 subject and prints grade according to the parameter.
#include <stdio.h>

int main() {
    int m1, m2, m3, m4, m5;
    int total;
    float percentage;

    printf("Enter marks of 5 subjects:\n");
    scanf("%d%d%d%d%d", &m1, &m2, &m3, &m4, &m5);

    total = m1 + m2 + m3 + m4 + m5;
    percentage = total / 5.0;

    printf("Percentage = %.2f\n", percentage);

    if (percentage >= 90)
        printf("Grade A");
    else if (percentage >= 75)
        printf("Grade B");
    else if (percentage >= 60)
        printf("Grade C");
    else if (percentage >= 40)
        printf("Grade D");
    else
        printf("Fail");

    return 0;
}
11-WAP to find even and odd numbers from 1 to n .
#include <stdio.h>

int main() {
    int n, i;

    printf("Enter the value of n: ");
    scanf("%d", &n);

    printf("Even numbers from 1 to %d are:\n", n);
    for(i = 1; i <= n; i++) {
        if(i % 2 == 0)
            printf("%d ", i);
    }

    printf("Odd numbers from 1 to %d are:\n", n);
    for(i = 1; i <= n; i++) {
        if(i % 2 != 0)
            printf("%d ", i);
    }

    return 0;
}
12-WAP to print Fibonacci series.
#include <stdio.h>

int main() {
    int n, i;
    int a = 0, b = 1, c;

    printf("Enter number of terms: ");
    scanf("%d", &n);

    printf("Fibonacci Series:\n");

    for(i = 1; i <= n; i++) {
        printf("%d ", a);

        c = a + b;
        a = b;
        b = c;
    }

    return 0;
}
13-WAP to make calculator using switch case.
5#include <stdio.h>

int main() {
    int a, b, choice;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    printf("Addition");
    printf("Subtraction");
    printf("Multiplication");
    printf("Division");

    printf("Enter your choice: ");
    scanf("%d", &choice);

    switch(choice) {
        case 1:
            printf("Sum = %d", a + b);
            break;

        case 2:
            printf("Difference = %d", a - b);
            break;

        case 3:
            printf("Product = %d", a * b);
            break;

        case 4:
            printf("Quotient = %d", a / b);
            break;

        default:
            printf("Invalid Choice");
    }

    return 0;
}
14-WAP to add and multiply two matrix of order n*n.
#include <stdio.h>

int main() {
    int n, i, j;
    
    printf("Enter order of matrix: ");
    scanf("%d", &n);

    int a[n][n], b[n][n], sum[n][n];

    printf("Enter elements of first matrix:\n");
    for(i = 0; i < n; i++) {
        for(j = 0; j < n; j++) {
            scanf("%d", &a[i][j]);
        }
    }

    printf("Enter elements of second matrix:\n");
    for(i = 0; i < n; i++) {
        for(j = 0; j < n; j++) {
            scanf("%d", &b[i][j]);
        }
    }

    for(i = 0; i < n; i++) {
        for(j = 0; j < n; j++) {
            sum[i][j] = a[i][j] + b[i][j];
        }
    }

    printf("Sum of matrices:\n");
    for(i = 0; i < n; i++) {
        for(j = 0; j < n; j++) {
            printf("%d ", sum[i][j]);
        }
        printf("\n");
15-WAP to reverse the number.
#include <stdio.h>

int main() {
    int num, reverse = 0, rem;

    printf("Enter a number: ");
    scanf("%d", &num);

    while(num != 0) {
        rem = num % 10;
        reverse = reverse * 10 + rem;
        num = num / 10;
    }

    printf("Reverse number = %d", reverse);

    return 0;
}
16-WAP to find sum of digits of entered number.
#include <stdio.h>

int main() {
    int num, sum = 0, rem;

    printf("Enter a number: ");
    scanf("%d", &num);

    while(num != 0) {
        rem = num % 10;
        sum = sum + rem;
        num = num / 10;
    }

    printf("Sum of digits = %d", sum);

    return 0;
}
17-WAP for passing elements in an array.
#include <stdio.h>

int main() {
    int arr[5], i;

    printf("Enter 5 elements:\n");

    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Array elements are:\n");

    for(i = 0; i < 5; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}
18-WAP to print sum of the elements of the array.
#include <stdio.h>

int main() {
    int arr[5], i, sum = 0;

    printf("Enter 5 elements:\n");

    for(i = 0; i < 5; i++) {
        scanf("%d", &arr[i]);
    }

    for(i = 0; i < 5; i++) {
        sum = sum + arr[i];
    }

    printf("Sum of array elements = %d", sum);

    return 0;
}
19-WAP to search element in an array using linear search.
#include <stdio.h>

int main() {
    int arr[10], i, n, key, found = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter array elements:\n");
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Enter element to search: ");
    scanf("%d", &key);

    for(i = 0; i < n; i++) {
        if(arr[i] == key) {
            found = 1;
            break;
        }
    }

    if(found == 1)
        printf("Element found at position %d", i + 1);
    else
        printf("Element not found");

    return 0;
}
20-WAP to sort an array using bubble sort.
#include <stdio.h>

int main() {
    int arr[10], n, i, j, temp;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    printf("Enter array elements:\n");
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for(i = 0; i < n - 1; i++) {
        for(j = 0; j < n - i - 1; j++) {
            if(arr[j] > arr[j + 1]) {
                temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }

    printf("Sorted array:\n");

    for(i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    return 0;
}

