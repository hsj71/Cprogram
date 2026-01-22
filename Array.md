# Insertion Operation 

```
1. Start 
2. Set J = N 
3. Set N = N+1 
4. Repeat steps 5 and 6 while J >= K 
5. Set LA[J+1] = LA[J] 
6. Set J = J-1 
7. Set LA[K] = ITEM 
8. Stop

```
---

```
#include <stdio.h> 
 
main() { 
   int LA[] = {1,3,5,7,8}; 
   int item = 10, k = 3, n = 5; 
   int i = 0, j = n; 
   printf("The original array elements are :\n"); 
   for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
   n = n + 1; 
   while( j >= k) { 
      LA[j+1] = LA[j]; 
      j = j - 1; 
   } 
   LA[k] = item; 
   printf("The array elements after insertion :\n"); 
   for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
} 

```
---
# Deletion Operation 
```
1. Start 
2. Set J = K 
3. Repeat steps 4 and 5 while J < N 
4. Set LA[J] = LA[J + 1] 
5. Set J = J+1 
6. Set N = N-1 
7. Stop 
```
---
```
#include <stdio.h> 
 
void main() { 
   int LA[] = {1,3,5,7,8}; 
   int k = 3, n = 5; 
   int i, j; 
     printf("The original array elements are :\n"); 
   for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
     
   j = k; 
   while( j < n) { 
      LA[j-1] = LA[j]; 
      j = j + 1; 
   } 
   n = n -1; 
     printf("The array elements after deletion :\n"); 
   for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
} 
```
---
# Search Operation
```
1. Start 
2. Set J = 0 
3. Repeat steps 4 and 5 while J < N 
4. IF LA[J] is equal ITEM THEN GOTO STEP 6 
5. Set J = J +1 
6. PRINT J, ITEM 
7. Stop 
```
---
```
#include <stdio.h> 
 
void main() { 
   int LA[] = {1,3,5,7,8}; 
   int item = 5, n = 5; 
   int i = 0, j = 0; 
      printf("The original array elements are :\n"); 
    for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
     while( j < n){ 
      if( LA[j] == item ) { 
         break; 
      } 
     j = j + 1; 
   } 
  printf("Found element %d at position %d\n", item, j+1); 
}
```
---
# Update Operation
```
1. Start 
2. Set LA[K-1] = ITEM 
3. Stop 
```
---
```
#include <stdio.h> 
 
void main() { 
   int LA[] = {1,3,5,7,8}; 
   int k = 3, n = 5, item = 10; 
   int i, j; 
     printf("The original array elements are :\n"); 
   for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
     
   LA[k-1] = item; 
  printf("The array elements after updation :\n"); 
   for(i = 0; i<n; i++) { 
      printf("LA[%d] = %d \n", i, LA[i]); 
   } 
} 
```
---
# Sparse Matrix Using Array
```
#include<stdio.h> 
int main() 
{ 
  // Assume 4x5 sparse matrix 
  int sparseMatrix[4][5] = 
  { 
    {0 , 0 , 3 , 0 , 4 }, 
    {0 , 0 , 5 , 7 , 0 }, 
    {0 , 0 , 0 , 0 , 0 }, 
    {0 , 2 , 6 , 0 , 0 } 
  }; 
  int size = 0; 
  for (int i = 0; i < 4; i++) 
    for (int j = 0; j < 5; j++) 
      if (sparseMatrix[i][j] != 0) 
        size++; 
  int compactMatrix[3][size]; 
  // Making of new matrix 
  int k = 0; 
  for (int i = 0; i < 4; i++) 
    for (int j = 0; j < 5; j++) 
      if (sparseMatrix[i][j] != 0) 
      { 
        compactMatrix[0][k] = i; 
        compactMatrix[1][k] = j; 
        compactMatrix[2][k] = sparseMatrix[i][j]; 
        k++; 
      } 
  for (int i=0; i<3; i++) 
  { 
    for (int j=0; j<size; j++) 
      printf("%d ", compactMatrix[i][j]); 
      printf("\n"); 
  } 
  return 0; 
} 

```
---
```
0 0 1 1 3 3 
2 4 2 3 1 2 
3 4 5 7 2 6 
```
---
