EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:
```
int top;
char stack[100];
void display()
{
  if (top==-1)printf("stack is empty");
 for(int i=top;i>=0;i--)printf("%c ",stack[i]);
}
```
Output:

![Screenshot 2025-06-01 131218](https://github.com/user-attachments/assets/d47e506b-7fd4-4e4b-b448-b0d7452c1c24)


Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:
```
float stack[100];
int size=3,top=-1,i;
void push (float data)
{
  if (top==size-1)
  {printf("stack is full\n"); 
  return;}
  top++;
  stack[top]=data; 
}
```
Output:

![Screenshot 2025-06-01 131408](https://github.com/user-attachments/assets/8b95ec66-f9a9-4b27-b33c-ee80e6b1c078)

Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:
```
char queue[50];
int rear=-1, front=-1;
void display()
{
    if (front==-1)
    {
        printf("No elements to display");
        return ;
    }
    for (int i=front;i<=rear;i++)
    {
        printf("%c\n",queue[i]);
    }
}
```
Output:

![Screenshot 2025-06-01 131538](https://github.com/user-attachments/assets/73d39b55-239e-4ce8-b607-b89d7ba22569)

Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```
#define size 50
float queue[size];
int front = -1, rear = -1;

void enqueue(float data) {
    if (rear == size - 1) {
        printf("Queue is full\n");
        return;
    }
    if (front == -1) {
        front = 0;
    }
    rear++;
    queue[rear] = data;
}
```
Output:

![Screenshot 2025-06-01 131717](https://github.com/user-attachments/assets/e1c8dc48-8ba0-45e4-8cf9-9c1b08ee704a)


Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:
```
int front, rear;
void dequeue()
{
     if(front==-1||front>rear)printf("No elements to display\n"); 
     else 
     {
      front=front+1;
     }
    
}
```
Output:

![Screenshot 2025-06-01 131851](https://github.com/user-attachments/assets/eb674fd2-9a12-4e61-b287-5986e0e08965)



Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
