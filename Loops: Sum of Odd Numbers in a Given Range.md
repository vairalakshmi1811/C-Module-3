# Loops: Sum of Odd Numbers in a Given Range

This project contains a simple **C program** that calculates the **sum of all odd numbers** within a user-defined range using a **`for` loop**.

## 🧠 Aim

To write a C program that finds and sums all odd numbers in a specified range using a `for` loop.

## 📋 Algorithm

1. Declare integer variables: `n`, `m`, `i`, and `sum`. Initialize `sum = 0`.
2. Prompt the user to enter the starting (`m`) and ending (`n`) values of the range.
3. Use a `for` loop to iterate from `m` to `n - 1`.
4. Inside the loop:
   - Check if the current number `i` is odd (`i % 2 != 0`).
   - If odd, print `i` and add it to `sum`.
5. After the loop, display the total `sum` of the odd numbers.
6. Return `0` to indicate successful execution.

## 💻 Program
```
#include <stdio.h>

int main() {
    int n, m, i, sum = 0;
    printf("Enter the starting value (m): ");
    scanf("%d", &m);

    printf("Enter the ending value (n): ");
    scanf("%d", &n);
    printf("Odd numbers in the range:\n");
    for(i = m; i < n; i++) {
        if(i % 2 != 0) {
            printf("%d ", i);
            sum += i;
        }
    }
    printf("\nSum of odd numbers = %d\n", sum);

    return 0;
}
```
## Output
<img width="909" height="370" alt="image" src="https://github.com/user-attachments/assets/73de3782-896f-4236-abd6-d717999f0535" />

## Result
 C program that finds and sums all odd numbers in a specified range using a `for` loop is written.
