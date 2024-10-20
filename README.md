# EXPERIMENT 20

AIM:- To learn and implement sorting algorithms <br>

Software used:- VS code <br>

Theory:-<br>
Sorting algorithms arrange data in a particular order (ascending or descending) to make searching and processing more efficient. Common sorting algorithms include <br>

1).Bubble Sort: Repeatedly swaps adjacent elements if they are in the wrong order. It's simple but inefficient for large datasets (O(n²) time complexity).<br>
2).Selection Sort: Selects the smallest (or largest) element from the unsorted part and swaps it with the first unsorted element. Like Bubble Sort, it’s O(n²) in time complexity.<br>
3).Insertion Sort: Builds a sorted array one element at a time, inserting elements into their correct position. It’s efficient for small or partially sorted arrays with O(n²) complexity.<br>

CODE :-<br>

1).selction sort<br>
```
#include <iostream>
    #include <algorithm>
    using namespace std;
    // Selection sort
    int main() {
    int arr[5] = {10, 17, 27, 4, 6};
    int n = 5;

    for (int i = 0; i < n - 1; i++) {
        int min_index = i;
        for (int j = i + 1; j < n; j++) {
            if (arr[j] < arr[min_index]) { 
                min_index = j;             }
        }
        if (i != min_index) {
            swap(arr[i], arr[min_index]);
        }
    }

    cout << "The sorted array will be: ";
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";    }

    cout << endl;
    return 0;}
```
b.insertion sort
```
 #include <iostream>
    #include <algorithm>

    using namespace std;

    void selectionSort(int arr[], int n) {
    for (int i = 0; i < n - 1; i++) {
        int min_index = i;
        for (int j = i + 1; j < n; j++) {
            if (arr[j] < arr[min_index]) {
                min_index = j;
            }
        }
        swap(arr[i], arr[min_index]);
    }
    }

    int main() {
    int arr[] = {64, 25, 12, 22, 11};
    int n = sizeof(arr) / sizeof(arr[0]);

    selectionSort(arr, n);

    cout << "Sorted array: ";
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
    }
```
c.bubble sort
```
#include <iostream>
    #include <algorithm>
    using namespace std;

    int main() {
    int arr[5] = {10, 17, 27, 4, 6};
    int n = 5;

    for (int i = 0; i < n; i++) {
        for (int j = 0; j < n - 1; j++) { 
            if (arr[j] > arr[j + 1]) { 
                swap(arr[j], arr[j + 1]); 
            }
        }
    }

    cout << "The sorted array will be: ";
    for (int i = 0; i < n; i++) {
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
    }
```
## OUTPUT
exp 1
![image](https://github.com/user-attachments/assets/d5282c28-54e2-44ea-b5e9-87ae7df8bcd1)

exp 2 
![image](https://github.com/user-attachments/assets/03d87f26-4fdf-4159-b21c-40d849b4ac76)

exp 3
![image](https://github.com/user-attachments/assets/2bb48479-433a-4080-b93c-3de844490542)
## CONCLUSION
in this experiment we learnt about the sorting algorithms.
