# 1: Find Largest and Smallest Number Among 4 Numbers

## FlowChart

<img src="assets\1.png" alt="Flowchart Image" width="400"/>


## 🔸 Code Flow (Step-by-Step Logic)

1. Prompt user to enter 4 integers  
2. Store them in variables `a`, `b`, `c`, `d`  
3. Initialize `max` and `min` with `a`  
4. Use conditional checks to compare `b`, `c`, and `d` to update both `max` and `min`  
5. Display the result  

---

## 🔸 C Code Example

```c
#include <stdio.h>

int main() {
    int a, b, c, d, max, min;

    printf("Enter 4 numbers:\n");
    scanf("%d %d %d %d", &a, &b, &c, &d);

    max = min = a;

    if (b > max) max = b;
    if (b < min) min = b;

    if (c > max) max = c;
    if (c < min) min = c;

    if (d > max) max = d;
    if (d < min) min = d;

    printf("Largest = %d\n", max);
    printf("Smallest = %d\n", min);

    return 0;
}
