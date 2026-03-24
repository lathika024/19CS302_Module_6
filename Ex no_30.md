# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.
## DATE:
## AIM:
To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm
Start. Declare array size Initialize array elements using malloc() Update array size using realloc() Print the result. End.

## Program:
```
/*
C program to add two integer elements in an array using realloc() and that array already has three elements.

#include <stdio.h>
#include <stdlib.h>
int main() {
 int *arr, size, i;
 size = 3;
 arr = (int *)malloc(size * sizeof(int)); 
 for (i = 0; i < size; i++) {
 arr[i] = i * 10; }
 printf("Original array:\n");
 for (i = 0; i < size; i++) {
 printf("%d ", arr[i]);
 }
 printf("\n");
 size *= 2;
 arr = (int *)realloc(arr, size * sizeof(int)); 
 for (i = size / 2; i < size; i++) {
 arr[i] = i * 10;
printf("Updated array:\n");
 for (i = 0; i < size; i++) {
 printf("%d ", arr[i]);
 }}
*/
```

## Output:

<img width="458" height="233" alt="515540423-e48b1cae-6275-4c65-b91e-cd21385568ba" src="https://github.com/user-attachments/assets/ed66093c-88ca-43aa-8879-437321f3fb00" />

## Result:
Thus the program was executed and the output was verified successfully.
