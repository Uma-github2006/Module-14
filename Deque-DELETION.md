# Exp.No:38  
## Deque - DELETION


### AIM  
To write a Python program to delete elements at FRONT END of deque using a collection built-in function.


### ALGORITHM  

1. Import the `deque` class from the `collections` module.  
2. Create an empty deque.  
3. Define how many elements to input (e.g., 3 inputs as in the example).  
4. Loop through the range of input size:  
   - Read an integer from the user.  
   - Append the integer to the deque.  
5. Remove the front element of the deque using `popleft()`.  
6. Print the final deque after deletion.  

### PROGRAM  

```
import collections
a=int(input())
b=int(input())
c=int(input())
d=collections.deque([a,b,c])
d.popleft()
print("The deque after deleting is :")
print(d)

```

### OUTPUT
![image](https://github.com/user-attachments/assets/2a8496a4-d004-4a77-9bc0-2c9d3fab4a49)




### RESULT
Thus the Python program to delete elements at FRONT END of deque using a collection built-in function is executed successfully.
