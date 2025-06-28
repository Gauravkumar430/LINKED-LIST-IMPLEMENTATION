# LINKED-LIST-IMPLEMENTATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: GAURAV KUMAR

*INTERN ID*: CT04DF963

*DOMAIN*: C PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH

*DESCRIPTION*: A Singly Linked List (SLL) is a linear data structure composed of elements called nodes, where each node contains two parts:

Data: The actual value stored.

Pointer (next): A link to the next node in the sequence.

Unlike arrays, linked lists do not require contiguous memory locations. They are dynamic and can grow or shrink during runtime.

🔹 Structure of Node
The fundamental unit in the program is the struct Node, which contains an integer data and a pointer next pointing to the next node.

c
Copy
Edit
struct Node {
    int data;
    struct Node* next;
};
🔹 Node Creation
The createNode() function dynamically allocates memory for a new node and initializes it with the given data value.

🔹 Insertion Operation
The insertEnd() function adds a new node at the end of the list.

If the list is empty (*head == NULL), the new node becomes the head.

Otherwise, the function iterates to the last node (while (temp->next != NULL)) and links the new node.

This allows users to keep appending new data as the list grows.

🔹 Deletion Operation
The deleteNode() function removes the first node that matches a given value.

It first checks if the list is empty.

If the value is at the head, it adjusts the head pointer and frees the node.

Otherwise, it searches for the node and adjusts pointers to unlink and delete it.

This prevents memory leaks and ensures correct linkage after deletion.

🔹 Traversal Operation
The traverse() function iterates over the list from the head to the end (head != NULL) and prints each node's value followed by ->. The output ends with NULL, indicating the end of the list.

🔹 Menu-Driven Interface
The main() function provides a user interface using a while loop with a switch-case structure.

The user can choose to insert, delete, traverse, or exit.

Input is taken using scanf and passed to the respective function.

This modular design separates concerns: each functionality (insert, delete, display) is implemented as a separate function, making the code more readable, maintainable, and reusable.

🔹 Memory Management
Each node is dynamically allocated using malloc, and deleted using free. This ensures memory is used efficiently and can be reclaimed when no longer needed.

 Advantages of This Modular Implementation
Efficiency: Each operation (insertion, deletion, traversal) is optimized with minimal overhead.

Modularity: Functions are well-structured and reusable.

Flexibility: Easily extendable to include features like insertion at position, reverse traversal, etc.

Clarity: The code is clean and easy to understand for both beginners and intermediate learners.

*OUTPUT*:

