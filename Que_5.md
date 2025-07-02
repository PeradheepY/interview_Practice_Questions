## 5. Write a C program to print the following number pattern based on **user input** for the number of rows:

### Example (for rows = 4):

```
1
1 2 3
1 2 3 4 5
1 2 3 4 5 6 7
```


---

## Flowchart

<img src="assets\5.png" alt="Flowchart Image" width="400"/>

---

## Code Flow (Logic Steps)

1. Start the program  
2. Take number of rows `n` as input from user  
3. For `i = 1` to `n`:
   - Loop `j = 1` to `2*i - 1`:
     - Print `j`
   - Print a newline
4. End the program

---

## C Code

```c
#include <stdio.h>

int main() {
    int i, j, rows;

    // Get number of rows from user
    printf("Enter number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= 2 * i - 1; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }

    return 0;
}
