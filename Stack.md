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
## Postfix Evaluation Algorithm 
Assume we have a string of operands and operators, an informal, by hand process is 
```
1. Scan the expression left to right 
2. Skip  values or variables (operands) 
3. When an operator is found, apply the operation to the preceding two operands 
4. Replace the two operands and operator with the calculated value (three symbols are 
replaced with one operand) 
5. Continue scanning until only a value remains--the result of the expression
```
The time complexity is O(n) because each operand is scanned once, and each operation is 
performed once. 
```
create a new stack 
while(input stream is not empty){ 
   token = getNextToken(); 
   if(token instanceof operand){ 
      push(token); 
   } else if (token instance of operator) {
      op2 = pop(); 
      op1 = pop(); 
      result = calc(token, op1, op2); 
      push(result); 
   } 
} 
return pop();
```
Demonstration with 2 3 4 + * 5 -  is 2 7 * 5 - then 14 5 - then 9

---
# Memory Management 
## When a method/function is called 
```
1. An activation record is created; its size depends on the number and size of the local 
variables and parameters. 
2. The Base Pointer value is saved in the special location reserved for it 
3. The Program Counter value is saved in the Return Address location 
4. The Base Pointer is now reset to the new base (top of the call stack prior to the creation 
of the AR) 
5. The Program Counter is set to the location of the first bytecode of the method being 
called 
6. Copies the calling parameters into the Parameter region 
7. Initializes local variables in the local variable region
```
While the method executes, the local variables and parameters are simply found by adding a 
constant associated with each variable/parameter to the Base Pointer. 
When a method returns 
```
1. Get the program counter from the activation record and replace what's in the PC 
2. Get the base pointer value from the AR and replace what's in the BP 
3. Pop the AR entirely from the stack. 
```
---
# Infix to Postfix Conversion  
```
#include<stdio.h> 
char stack[20]; 
int top = -1; 
void push(char x) 
{ 
    stack[++top] = x; 
} 
  
char pop() 
{ 
    if(top == -1) 
        return -1; 
    else 
        return stack[top--]; 
} 
  
int priority(char x) 
{ 
    if(x == '(') 
        return 0; 
    if(x == '+' || x == '-') 
        return 1; 
    if(x == '*' || x == '/') 
        return 2; 
} 
  
main() 
{ 
    char exp[20]; 
    char *e, x; 
    printf("Enter the expression :: "); 
    scanf("%s",exp); 
    e = exp; 
    while(*e != '\0') 
    { 
        if(isalnum(*e)) 
            printf("%c",*e); 
        else if(*e == '(') 
            push(*e); 
        else if(*e == ')') 
        { 

            while((x = pop()) != '(') 
                printf("%c", x); 
        } 
        else 
        { 
            while(priority(stack[top]) >= priority(*e)) 
                printf("%c",pop()); 
            push(*e); 
        } 
        e++; 
    } 
    while(top != -1) 
    { 
        printf("%c",pop()); 
    } 
} 
```
---
OUTPUT: 
```
Enter the expression :: a+b*c 
abc*+ 
 
Enter the expression :: (a+b)*c+(d-a) 
ab+c*da-+
```
---
# Evaluate POSTFIX Expression Using Stack
```
#include<stdio.h> 
int stack[20]; 
int top = -1; 
 void push(int x) 
{ 
        stack[++top] = x; 
} 
  
int pop() 
{ 
        return stack[top--]; 
} 
  
int main() 
{ 
        char exp[20]; 
        char *e; 
        int n1,n2,n3,num; 
        printf("Enter the expression :: "); 
        scanf("%s",exp); 
        e = exp; 
        while(*e != '\0') 
        { 
                if(isdigit(*e))
                {     num = *e - 48;   // 48 == '0' as all stored *e+48 in ascii
                      push(num); 
                } 
                else {  n1 = pop(); 
                        n2 = pop(); 
                        switch(*e) 
                        { 
                                case '+': 
                                { 
                                        n3 = n1 + n2; 
                                         break; 
                                } 
                                case '-': 
                                { 
                                        n3 = n2 - n1; 
                                        break; 
                                } 
                                case '*': 
                                { 
                                        n3 = n1 * n2; 
                                        break; 
                                }
                                case '/': 
                                { 
                                        n3 = n2 / n1; 
                                        break; 
                                } 
                        } 
                        push(n3); 
                } 
                e++; 
        } 
        printf("\nThe result of expression %s  =  %d\n\n",exp,pop()); 
        return 0; 
}
```
```
Output: 
Enter the expression :: 245+* 
The result of expression 245+*  =  18
```
---
