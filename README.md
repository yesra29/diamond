# diamond
#include <stdio.h>

int main() {
    int rows, i, j, space;

    // Get the number of rows from the user
    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    // Upper part of the diamond
    for (i = 1; i <= rows; i++) {
        // Loop to print spaces before the '*'
        for (space = 1; space <= rows - i; space++) {
            printf(" ");
        }
        // Loop to print '*' in each row
        for (j = 1; j <= 2 * i - 1; j++) {
            printf("*");
        }
        // Move to the next line after each row is printed
        printf("\n");
    }

    // Lower part of the diamond
    for (i = rows - 1; i >= 1; i--) {
        // Loop to print spaces before the '*'
        for (space = 1; space <= rows - i; space++) {
            printf(" ");
        }
        // Loop to print '*' in each row
        for (j = 1; j <= 2 * i - 1; j++) {
            printf("*");
        }
        // Move to the next line after each row is printed
        printf("\n");
    }

    return 0;
}
