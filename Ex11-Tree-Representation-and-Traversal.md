# Ex11 Tree Representation and Traversal
## DATE:25/04/2025
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1.Start<br/>
2.Define a function display_postorder() that takes a pointer to the root node of the tree.<br/>
3.Check if the current node (root_node) is not null.<br/>
4.Recursively call display_postorder() for the left child of the current node.<br/>
5.Recursively call display_postorder() for the right child of the current node.<br/>
6.After visiting both children, print the value of the current node.<br/>
7.End<br/>

## Program:
```
/*
Program to perform post order traversal of a binary tree.
Developed by: T.KAVINAJAI
RegisterNumber: 212223100020
*/
struct node 
{ 
int value; 
struct node *left_child, *right_child; 
};*/ 
void display_postorder(struct node *root_node) { 
if(root_node) 
{ 
display_postorder(root_node->left_child); 
display_postorder(root_node->right_child); 
printf("%d\n",root_node->value); 
} 
} 
```
## Output:
![image](https://github.com/user-attachments/assets/a8366de1-d2a4-4e2d-a4b7-3dc058890c10)



## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
