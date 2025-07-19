# IDENTITY-MATRIX-IN-C
#include <stdio.h>

int main() {
    int size;
    printf("Enter the size of the identity matrix: ");
    scanf("%d", &size);

    int identity[100][100];  // You can use dynamic allocation for large sizes

    // Generating identity matrix
    for (int i = 0; i < size; i++) {
        for (int j = 0; j < size; j++) {
            if (i == j)
                identity[i][j] = 1;
            else
                identity[i][j] = 0;
        }
    }

    // Printing the matrix
    printf("Identity matrix of size %d:\n", size);
    for (int i = 0; i < size; i++) {
        for (int j = 0; j < size; j++) {
            printf("%d\t", identity[i][j]);
        }
        printf("\n");
    }

    return 0;
}
//
// Created by Suprakash Ghosh on 19-07-2025.
//
