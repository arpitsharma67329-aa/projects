#include <stdio.h>

int main() {
    int n, i, min;

    // Input: size of array
    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    int arr[n];  // declare array

    // Input: array elements
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Assume first element is minimum
    min = arr[0];

    // Compare with remaining elements
    for(i = 1; i < n; i++) {
        if(arr[i] < min) {
            min = arr[i];
        }
    }

    // Output: minimum value
    printf("Minimum value in the array is: %d\n", min);

    return 0;
}
