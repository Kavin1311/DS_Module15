# Ex14 Heap Tree
## DATE: 25/04/2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1.Start<br/>
2.Find the index of the element num in the array.<br/>
3.Swap the element to be deleted with the last element in the array.<br/>
4.Decrease the array size (size) by 1.<br/>
5.Start heapifying from the last non-leaf node (index size/2 - 1).<br/>
6.Call heapify() to restore the heap property for each node.<br/>
7.End<br/>

## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: T.KAVINAJAI
RegisterNumber:  212223100020
*/
void deleteRoot(int array[], int num) 
{ 
int i; 
for(i=0;i<size;i++) 
{ 
if(num==array[i]) 
{ 
break; 
} 
} 
swap(&array[i],&array[size-1]); 
size-=1; 
for(i=size/2-1;i>=0;i--) 
{ 
heapify(array,size,i); 
} 
}
```

## Output:
![image](https://github.com/user-attachments/assets/0862893a-8a09-4817-98fa-0cc89849be7b)



## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
