# 19CS301-Module10
###EX: 10.a  STACK
### Aim: 
To Write a python program to get the integer values from the user and push only the odd number into the stack and later pop the last 2 elements
### Algorithm:
STEP 1: Start.

STEP 2: Create a list and a variable n.

STEP 3: Get the value of n from user.

STEP 4: Using loop append only odd elements in the stack.

STEP 5 : Using another loop using built-in pop operation pop the last two elements.

STEP 6: Print the result.

STEP 7 : Stop.
### Program:
```
l = []
n = int(input())
for i in range(n):
       x = int(input())
       if x%2!=0:
            l.append(x)
 print(l)
for i in range(2):
      l.pop()
     print(l)
```
### Output:
 ![image](https://github.com/user-attachments/assets/d2ce0434-7594-41af-ba20-3d7ecf9e0d93)

### Result: Thus, the given program is implemented and executed successfully .
 


### EX: 10.2 IMPLEMENTATION OF STACK
### Aim: 
To Write a python program to implement the stack using deque method for rotating the stack.
### Algorithm:

STEP 1: Start.

STEP 2: Import collections and import deque.

STEP 3: Create a list and get the input from user.

STEP 4: Create a variable n and get number of inputs from user.

STEP 5 : Using a loop get the inputs from user and append in deque.

STEP 6: Using rotate function rotate the stack.

STEP 7 : Print the result. 

STEP 8 : Stop.
### Program: 
```
import collections
def fun(n):
   stack = collections.deque([])
   a=int(input())
   for i in range (a):
         x=stack.append(int(input()))
     print(f"Stack before rotation {stack}") stack.rotate(n)
print(f"Stack after rotation {stack}")
```
### Output:
![image](https://github.com/23013357/19CS301-Module10/blob/main/e.png)

### Result: Thus, the given program is implemented and executed successfully .
 


EX: 10.3 QUEUE
### Aim: 
To Write a python program to implement the stack using deque method for rotating the stack.
### Algorithm:

STEP 1: Start.

STEP 2: Import collections and import deque.

STEP 3: Create a stack and a variable n.

STEP 4: Get the number of inputs from user.

STEP 5: Using a loop get the inputs from user.

STEP 6: Append the even and unique elements in the stack.

STEP 7: Print the result.
### Program:
```
import collections
stack = collections.deque([])
n = int(input())
for i in range(n):
       x = int(input())
        if x not in stack:
          if x%2==0:
             stack.appendleft(x)
print(stack)
```
### Output:
![image](https://github.com/user-attachments/assets/de6e3e09-b10b-42d4-9faf-32fcf990f29a)
 
### Result: Thus, the given program is implemented and executed successfully .


### EX: 10.4 IMPLEMENTATION OF QUEUE
### Aim: 
To Develop a python program to get the 4 integer values from user and display the values using multiprocessing library
### Algorithm:

STEP 1: Start.

STEP 2: From Multiprocessing Import Queue.

STEP 3: Create a list and get the input from user.

STEP 4 : Append the elements in the list.

STEP 5: Using 'get' built-in function print the list.

STEP 6 : Print the result.

STEP 7 : Stop.
### Program:
```
from multiprocessing import Queue
queue = Queue()
for i in range(4):
    queue.put(int(input()))
for i in range(4):
     print(queue.get())
```
### Output:
 ![image](https://github.com/user-attachments/assets/26a380ff-118e-43f4-8178-83a5417262b5)
 

### Result: Thus, the given program is implemented and executed successfully .

### EX: 10.5 MUTIPROCESSING OF QUEUE
### Aim: 
To  python program to display the colors and the number of colors the user provided using multiprocessing library
### Algorithm:

Start.

Take n as input for the number of colors.

Append n colors entered by the user into the list colors.

Initialize a queue and add each color to the queue, incrementing the counter cnt.

Print the counter cnt (number of colors).

Retrieve and print each color from the queue.

Stop.
### Program:
```

from multiprocessing import Queue

colors=[]
cnt=0
queue=Queue()
n=int(input())
colours=[]
for i in range(n):
    colors.append(input())
for color in colors:
    queue.put(color)
    cnt+=1
print('count-',cnt)
for i in range(n):
    print(queue.get())
```
### Output:
 ![image](https://github.com/23013357/19CS301-Module10/blob/main/MODUL%2010.png)
 

### Result: Thus, the given program is implemented and executed successfully .
 

