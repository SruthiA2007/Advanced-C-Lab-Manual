***EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.***

**Aim:**
To write a C program to display stack elements using an array.
**Algorithm:**
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
**Program:**

```
#include <stdio.h>

#define MAX 100

float stack[MAX];
int top = -1;

void display() {
    if(top == -1) {
        printf("Stack is empty\n");
        return;
    }
    
    printf("Stack elements: ");
    for(int i = 0; i <= top; i++) {
        printf("%.1f\n", stack[i]);
    }
    printf("\n");
}
```

**Output:**

<img width="456" height="483" alt="image" src="https://github.com/user-attachments/assets/ee7c8222-40bc-455e-8229-7fe9ee0bf58d" />




**Result:**
Thus, the program to display stack elements using an array is verified successfully.
 

**EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.**
**Aim:**
To create a C program to push the given element in to a stack using array.
**Algorithm:**
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
**Program:**

```
#include <stdio.h>

#define SIZE 100

float stack[SIZE];
int top = -1;

void push(float val) {
    if(top == SIZE - 1) {
        printf("Stack overflow\n");
        return;
    }
    
    stack[++top] = val;
    printf("%.2f pushed to stack\n", val);
}
```

**Output:**

<img width="578" height="419" alt="image" src="https://github.com/user-attachments/assets/395587ef-1304-4a65-9193-cf6a09e73054" />




**Result:**
Thus, the program to push the given element in to a stack using array is verified successfully


 
***EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.***
**Aim:**
To write a C program to display queue elements using array

**Algorithm:**
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
**Program:**

```
#include <stdio.h>

#define MAX 100

char queue[MAX];
int rear = -1;
int front = -1;

void display() {
    if(front == -1) {
        printf("Queue is empty\n");
        return;
    }
    
    printf("Queue elements: ");
    for(int i = front; i <= rear; i++) {
        printf("%c ", queue[i]);
    }
    printf("\n");
}
```

**Output:**

<img width="580" height="439" alt="image" src="https://github.com/user-attachments/assets/63e6f87d-5a7f-46c9-b6e0-5768de8cfc39" />


**Result:**
Thus, the program to display queue elements using array is verified successfully.


 
**EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.**
**Aim:**
To write a C program to insert elements in queue using array.

**Algorithm:**
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

**Program:**

```
#include <stdio.h>

#define SIZE 100

float queue[SIZE];
int rear = -1;
int front = -1;

void enqueue(float val) {
    if(rear == SIZE - 1) {
        printf("Queue overflow\n");
        return;
    }
    
    if(front == -1) {
        front = 0;
    }
    
    queue[++rear] = val;
    printf("%.1f inserted to queue\n", val);
}
```

**Output:**

<img width="582" height="342" alt="image" src="https://github.com/user-attachments/assets/81906cc1-7967-4525-9cee-59f5e85702e6" />


**Result:**
Thus, the program to insert elements in queue using array is verified successfully.



 
**EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY**



**Aim:**

To create a function in C that deletes an element from a queue implemented using an array.

**Algorithm:**

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



**Program:**

```
#include <stdio.h>

#define MAX 100

int queue[MAX];
int rear = -1;
int front = -1;

void dequeue() {
    if(front == -1) {
        printf("Queue is empty\n");
        return;
    }
    
    front++;
    
    if(front > rear) {
        front = rear = -1;
    }
}
```

**Output:**

<img width="580" height="677" alt="image" src="https://github.com/user-attachments/assets/cdf700f1-7fc4-47a5-92f4-2359d7368db1" />



**Result:**
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
