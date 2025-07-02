## 4. Write a C program to **swap two numbers without using a temporary variable**.

---

## Flowchart

<img src="assets\4.png" alt="Flowchart Image" width="400"/>

---

## Code Flow (Logic Steps)

1. Start the program  
2. Read two integers `a` and `b` from the user  
3. Swap using arithmetic operations:
   - `a = a + b`
   - `b = a - b` (now `b` has the original value of `a`)
   - `a = a - b` (now `a` has the original value of `b`)  
4. Print the swapped values  
5. End the program

---

## 💻 C Code

```c
#include <stdio.h>

int main() {
    int a, b;

    // Get input from user
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Display original values
    printf("Before swap: a = %d, b = %d\n", a, b);

    // Swap without temp variable
    a = a + b;
    b = a - b;
    a = a - b;

    // Display swapped values
    printf("After swap: a = %d, b = %d\n", a, b);

    return 0;
}
