#include <stdio.h>

int main() {
    int num1, num2;
    int addition, subtraction, multiplication;
    float division;
    int modulo;

    
    printf("Enter the first integer: ");
    scanf("%d", &num1);
    printf("Enter the second integer: ");
    scanf("%d", &num2);

   
    addition = num1 + num2;

  
    subtraction = num1 - num2;

   
    multiplication = num1 * num2;

    
    if (num2 != 0) {
        division = (float)num1 / num2;
    } else {
        printf("Error: Division by zero is not allowed.\n");
        division = 0; // Set a default value for division
    }

    
    if (num2 != 0) {
        modulo = num1 % num2;
    } else {
        printf("Error: Modulo by zero is not allowed.\n");
        modulo = 0; // Set a default value for modulo
    }

  
    printf("Addition: %d + %d = %d\n", num1, num2, addition);
    printf("Subtraction: %d - %d = %d\n", num1, num2, subtraction);
    printf("Multiplication: %d * %d = %d\n", num1, num2, multiplication);
    if (num2 != 0) {
        printf("Division: %d / %d = %.2f\n", num1, num2, division);
    }
    if (num2 != 0) {
        printf("Modulo: %d %% %d = %d\n", num1, num2, modulo);
    }

    return 0;
}
