#include <stdio.h>

int main() {
    int num1, num2;
    int sum, difference, product, remainder;
    float quotient;

    // Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &num1, &num2);

    // Perform arithmetic operations
    sum = num1 + num2;
    difference = num1 - num2;
    product = num1 * num2;

    // Check for division by zero
    if (num2 != 0) {
        quotient = (float)num1 / num2;  // typecast to float for decimal result
        remainder = num1 % num2;
    } else {
        printf("Division and modulus by zero are not allowed.\n");
        return 1;
    }

    // Display results
    printf("\nResults:\n");
    printf("Sum = %d\n", sum);
    printf("Difference = %d\n", difference);
    printf("Product = %d\n", product);
    printf("Quotient = %.2f\n", quotient);
    printf("Remainder = %d\n", remainder);

    return 0;
}
