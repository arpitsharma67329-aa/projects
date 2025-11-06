#include <stdio.h>
void selectionSort(int arr[], int n);
int main() {
    int arr[] = {5, 12, 14, 16, 17, 21, 15, 4, 3, 0};
    int n = 10, target = 15, found = 0;
    selectionSort(arr, n);
    printf("Sorted array: ");
    for(int i = 0; i < n; i++)
        printf("%d ", arr[i]);
    printf("\n");
    // Linear search
    for(int i = 0; i < n; i++) {
        if(arr[i] == target) {
            printf("Element %d found at index %d\n", target, i);
            found = 1;
            break;
        }
    }
    if(!found)
        printf("Element %d not found in array\n", target);
    return 0;
}
void selectionSort(int arr[], int n) {
    for(int i = 0; i < n-1; i++) {
        int min_idx = i;
        for(int j = i+1; j < n; j++)
            if(arr[j] < arr[min_idx])
                min_idx = j;
        int temp = arr[min_idx]; arr[min_idx] = arr[i]; arr[i] = temp;
    }
}
