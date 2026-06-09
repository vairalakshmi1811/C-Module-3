# Fuctions: EMI Calculator in C (Function Without Return Type With Arguments)

This repository contains a **C program** to calculate the **Equated Monthly Installment (EMI)** using a function that has **no return type but accepts arguments**.

## 🎯 Aim

To write a C program that calculates the EMI for a loan using a function **without return type and with arguments**.

## 📋 Algorithm

1. Start the program.
2. Read input values from the user:
   - Principal amount (`p`)
   - Rate of interest (`r`)
   - Loan duration in months (`t`)
3. Pass these values as arguments to a function.
4. Inside the function, calculate the EMI using the formula:
5. EMI = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1)

 Note: Ensure the rate `r` is converted to a monthly rate (i.e., divide annual rate by 12 * 100).

5. Display the EMI result.
6. Stop the program.

## 🧾Program
```
#include <stdio.h>
#include <math.h>
void calculateEMI(float p, float r, int t) {
    float emi;
    r = r / (12 * 100);
    emi = (p * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
    printf("EMI = %.2f\n", emi);
}

int main() {
    float p, r;
    int t;
    printf("Enter principal amount: ");
    scanf("%f", &p);

    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &r);

    printf("Enter loan duration (in months): ");
    scanf("%d", &t);
    calculateEMI(p, r, t);

    return 0;
}
```
## Sample Output
<img width="905" height="339" alt="image" src="https://github.com/user-attachments/assets/a33b61ba-3611-4250-829e-301138035786" />

## Result
C program that calculates the EMI for a loan using a function **without return type and with arguments** is written.
