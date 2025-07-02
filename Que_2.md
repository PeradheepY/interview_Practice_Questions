## 2. Print the number series:  

`1 2 3 6 5 10 7 14 9 18 11`


## Flowchart

<img src="assets\2.png" alt="Flowchart Image" width="400"/>

---

##  Code Flow (Logic Steps)

1. Start with `i = 1` (first odd number)
2. Initialize `count = 0`
3. While `count < 11`:
   - Print `i` (odd)
   - Increment `count`
   - If `count < 11`, print `2*i` (even)
   - Increment `count`
   - Increment `i` by 2 to get the next odd number

---

## C Code

```c
#include <stdio.h>

int main() {
    int i = 1;       
    int count = 0;   
    int limit = 11;  

    while (count < limit) {
        printf("%d ", i);       
        count++;

        if (count < limit) {    
            printf("%d ", 2 * i); 
            count++;
        }

        i += 2;  
    }

    return 0;
}
