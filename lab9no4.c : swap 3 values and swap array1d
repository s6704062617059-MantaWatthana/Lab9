#include <stdio.h>

// function prototype
void swapValue(int *a, int *b, int *c);
void swapArray(int a[], int b[], int size);

int main() {

    int a = 1, b = 2, c = 3;

    printf("Before swapValue: a=%d, b=%d, c=%d\n", a, b, c);
    swapValue(&a, &b, &c);
    printf("After swapValue: a=%d, b=%d, c=%d\n\n", a, b, c);

    int arr1[] = {1, 2, 3, 4, 5};
    int arr2[] = {10, 20, 30, 40, 50};
    int size = 5;

    printf("Before swapArray:\n");
    printf("arr1: ");
    for(int i = 0; i < size; i++)
        printf("%d ", arr1[i]);

    printf("\narr2: ");
    for(int i = 0; i < size; i++)
        printf("%d ", arr2[i]);

    swapArray(arr1, arr2, size);

    printf("\n\nAfter swapArray:\n");
    printf("arr1: ");
    for(int i = 0; i < size; i++)
        printf("%d ", arr1[i]);

    printf("\narr2: ");
    for(int i = 0; i < size; i++)
        printf("%d ", arr2[i]);

    return 0;
}

void swapValue(int *a, int *b, int *c) {

    int temp = *a;
    *a = *b;
    *b = *c;
    *c = temp;
}

void swapArray(int a[], int b[], int size) {

    for(int i = 0; i < size; i++) {
        int temp = a[i];
        a[i] = b[i];
        b[i] = temp;
    }
}
