# Ex13 Expression Tree
## DATE:25/04/2025
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1.Start<br/>
2.Print node data in preorder then traverse left then <br/>
3.Traverse left in inorder then print node data then traverse right<br/>
4.Traverse left in postorder then traverse right then print node data<br/>
5.Recursive approach is used for all three traversal methods<br/>
6.Functions handle each tree node using tree->d, tree->l, tree->r<br/>
7.End<br/>

## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: T.KAVINAJAI
RegisterNumber: 212223100020 
*/
struct n { 
char d; 
struct n *l; 
struct n *r; 
};*/ 
void preOrder(struct n *tree) 
{ 
if(tree) 
{ 
printf("%c",tree->d); 
preOrder(tree->l); 
preOrder(tree->r); 
} 
} 
void inOrder(struct n *tree) 
{ 
if(tree) 
{ 
inOrder(tree->l); 
printf("%c",tree->d); 
inOrder(tree->r); 
} 
} 
void postOrder(struct n *tree) 
  
  
{ 
if(tree) 
{ 
postOrder(tree->l); 
postOrder(tree->r); 
printf("%c",tree->d); 
} 
} 
```
## Output:

![image](https://github.com/user-attachments/assets/bb84060f-0ca9-4de4-b37f-92152fb3d8e7)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
