# Exp No: 36  
## Circular Queue 

### AIM  
To write a Python program with a function to insert float values into a Circular Queue.

### ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End



### PROGRAM

```
class Queue:
    def __init__(self,limit):
        self.queue=[]
        self.rear=0
        self.front=0
        self.limit=limit
    def isempty(self):
        if len(self.queue)==0:
            return True
        else:
            return False
    def enqueue(self,item):
        if len(self.queue) == self.limit:
            print("full")
        else:
            if self.rear == self.limit:
                self.rear =0
            self.queue.insert(self.rear,item)
            self.rear += 1
        
    def dequeue(self):
        if len(self.queue) ==0:
            print("under flow")
        else:
            if self.front == self.limit:
                self.front = 0
            self.queue.pop(self.front)
            self.front += 1
            
    def display(self):
        print(self.queue)
size =int(input())
q = Queue(size)
a=float(input())
b=float(input())
c=float(input())
q.enqueue(a)
q.enqueue(b)
q.enqueue(c)
q.display()
q.dequeue()
q.display()

```

### OUTPUT
![image](https://github.com/user-attachments/assets/83c0c871-26a0-4c36-9ef4-f39a59d78bed)



### RESULT
Thus the Python program with a function to insert float values into a Circular Queue is executed successfully.
