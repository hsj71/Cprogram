# Stack ----- LIFO

## peek() 
Algorithm of peek() function
```
begin procedure peek 
   return stack[top] 
end procedure 
```
```
int peek() { 
   return stack[top]; 
} 
```
---

## isfull() 
Algorithm of isfull() function − 
```
begin procedure isfull 
 
   if top equals to MAXSIZE 
      return true 
   else 
      return false 
   endif 
    
end procedure 
```
```
bool isfull() { 
   if(top == MAXSIZE) 
      return true; 
   else 
      return false; 
} 
```
---

## isempty() 
Algorithm of isempty() function − 
```
begin procedure isempty 
 
   if top less than 1 
      return true 
   else 
      return false 
   endif 
    
end procedure 
```
```
bool isempty() { 
   if(top == -1) 
      return true; 
   else 
      return false; 
} 
```
---

## Push Operation 
The process of putting a new data element onto stack is known as a Push Operation. Push 
operation involves a series of steps − 
```
 Step 1 − Checks if the stack is full. 
 Step 2 − If the stack is full, produces an error and exit. 
 Step 3 − If the stack is not full, increments top to point next empty space. 
 Step 4 − Adds data element to the stack location, where top is pointing. 
 Step 5 − Returns success. 
 ```
If the linked list is used to implement the stack, then in step 3, we need to allocate space 
dynamically. 
```
begin procedure push: stack, data 
 
   if stack is full 
return null 
endif 
top ← top + 1 
stack[top] ← data 
end procedure 
```
```
void push(int data) { 
if(!isFull()) { 
  top = top + 1;    
  stack[top] = data; 
} else { 
  printf("Could not insert data, Stack is full.\n"); 
  } 
} 
```
---

## Pop Operation 
Accessing the content while removing it from the stack, is known as a Pop Operation. In an 
array implementation of pop() operation, the data element is not actually removed, 
instead top is decremented to a lower position in the stack to point to the next value. But in 
linked-list implementation, pop() actually removes data element and deallocates memory space. 

```
Step 1 − Checks if the stack is empty. 
Step 2 − If the stack is empty, produces an error and exit. 
Step 3 − If the stack is not empty, accesses the data element at which top is pointing. 
Step 4 − Decreases the value of top by 1. 
Step 5 − Returns success. 
```
```
begin procedure pop: stack 
 
   if stack is empty 
      return null 
   endif 
    
   data ← stack[top] 
   top ← top - 1 
   return data 
 
end procedure 
```
```
int pop(int data) { 
 
   if(!isempty()) { 
      data = stack[top]; 
      top = top - 1;    
      return data; 
   } else { 
      printf("Could not retrieve data, Stack is empty.\n"); 
   } 
} 
```
---

# Stack Applications
<pre>
1. Expression evaluation 
2. Backtracking (game playing, finding paths, exhaustive searching) 
3. Memory management, run-time environment for nested language features. 
</pre>
---
| Infix Expression    | Prefix Expression   | Postfix Expression  |
| ------------------- | ------------------- | ------------------- |
| `a + b`             | `+ a b`             | `a b +`             |
| `a + b * c`         | `+ a * b c`         | `a b c * +`         |
| `(a + b) * (c - d)` | `* + a b - c d`     | `a b + c d - *`     |
| `b * b - 4 * a * c` | `- * b b * 4 * a c` | `b b * 4 a * c * -` |
| `40 - 3 * 5 + 1`    | `+ - 40 * 3 5 1`    | `40 3 5 * - 1 +`    |

---

