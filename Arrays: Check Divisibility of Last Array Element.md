# Arrays: Check Divisibility of Last Array Element

This repository contains a simple **C program** that reads `n` elements into an array and checks whether the **last element** is divisible by 2.

## 🧠 Aim

To create a C program that reads `n` integers into an array and determines if the **last element** is divisible by 2.

## 📋 Algorithm

1. Declare variables `n`, `i`, and an integer array `a[10]`.
2. Prompt the user to enter the value of `n` (number of elements).
3. Prompt: "The last element".
4. Read `n` elements into the array `a`.
5. Print the last element of the array.
6. Check if the last element (`a[n-1]`) is divisible by 2:
   - If true, print a message indicating it is divisible.
   - Otherwise, print a message that it is not divisible.
7. Return `0` to indicate successful execution.

## 🧾 Program
```
#include <stdio.h>
int main() {
    int n, i;
    int a[10];
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &a[i]);
    }
    printf("The last element is: %d\n", a[n-1]);
    if(a[n-1] % 2 == 0) {
        printf("The last element is divisible by 2.\n");
    } else {
        printf("The last element is not divisible by 2.\n");
    }

    return 0;
}
```

## Sample Output
<img width="905" height="446" alt="image" src="https://github.com/user-attachments/assets/6a54a6b8-ad60-45b8-b4c6-ff904cee9eea" />

## Result
 a C program that reads `n` integers into an array and determines if the **last element** is divisible by 2 is created
