## 3. Write a C program to **find the Least Common Multiple (LCM)** of two numbers entered by the user.
---

## Flowchart

<img src="assets\3.png" alt="Flowchart Image" width="400"/>

---

## Code Flow (Logic Steps)

1. Start the program
2. Read two numbers `a` and `b` from the user
3. Initialize `max` as the greater of `a` and `b`
4. Loop from `max` onwards:
   - If `max` is divisible by both `a` and `b`, then it's the LCM
   - Break the loop
   - Otherwise, increment `max` by 1
5. Print the LCM
6. End the program

---

## C Code

```c
#include <stdio.h>

int main() {
    int a, b, max;


    printf("Enter two positive integers: ");
    scanf("%d %d", &a, &b);

   
    max = (a > b) ? a : b;

    
    while (1) {
        if (max % a == 0 && max % b == 0) {
            printf("LCM of %d and %d is %d\n", a, b, max);
            break;
        }
        max++;
    }

    return 0;
}
