# QUEUE ------- FIFO

## peek() 
This function helps to see the data at the front of the queue. The algorithm of peek() function is 
```
begin procedure peek 
   return queue[front] 
end procedure
```
```
int peek() { 
   return queue[front]; 
}
```

## isfull() 
```
begin procedure isfull 
 
   if rear equals to MAXSIZE 
      return true 
   else 
      return false 
   endif 
    
end procedure
```
```
bool isfull() { 
   if(rear == MAXSIZE - 1) 
      return true; 
   else 
      return false; 
} 
```

## isempty() 
```
begin procedure isempty 
 
   if front is less than MIN  OR front is greater than rear 
      return true 
else 
return false 
endif 
end procedure
```
```
bool isempty() { 
if(front < 0 || front > rear)  
return true; 
else 
return false; 
}
```
---
## Enqueue Operation 
Queues maintain two data pointers, front and rear. Therefore, its operations are comparatively 
difficult to implement than that of stacks. 
```
Step 1 − Check if the queue is full. 
Step 2 − If the queue is full, produce overflow error and exit. 
Step 3 − If the queue is not full, increment rear pointer to point the next empty space. 
Step 4 − Add data element to the queue location, where the rear is pointing. 
Step 5 − return success.
```
```
procedure enqueue(data)       
if queue is full 
return overflow 
   endif 
    
   rear ← rear + 1 
   queue[rear] ← data 
   return true 
    
end procedure
```
```
int enqueue(int data)       
   if(isfull()) 
      return 0; 
    
   rear = rear + 1; 
   queue[rear] = data; 
    
   return 1; 
end procedure
```
--- 
##  Dequeue Operation 
Accessing data from the queue is a process of two tasks − access the data where front is 
pointing and remove the data after access. 
```
 Step 1 − Check if the queue is empty. 
 Step 2 − If the queue is empty, produce underflow error and exit. 
 Step 3 − If the queue is not empty, access the data where front is pointing. 
 Step 4 − Increment front pointer to point to the next available data element. 
 Step 5 − Return success. 
 
```
```
procedure dequeue 
    
   if queue is empty 
      return underflow 
   end if 
 
   data = queue[front] 
   front ← front + 1 
   return true 
 
end procedure
```
```
int dequeue() { 
   if(isempty()) 
      return 0; 
 
   int data = queue[front]; 
   front = front + 1; 
 
   return data; 
}
```
---
