#include <stdio.h>
int main() {
    int arr[] = {6, 7, 8, 9, 12, 14, 15, 18, 19, 20, 21};
    int n = 11, target = 18;
    int left = 0, right = n - 1, found = 0;
    while(left <= right) {
        int mid = left + (right - left) / 2;
        if(arr[mid] == target) {
            printf("Element %d found at index %d\n", target, mid);
            found = 1;
            break;
        }
        if(arr[mid] < target)
            left = mid + 1;
        else
            right = mid - 1;
    }
    if(!found)
        printf("Element %d not found in array\n", target);
    return 0;
}
