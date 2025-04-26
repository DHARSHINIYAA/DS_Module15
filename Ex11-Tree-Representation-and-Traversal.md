# Ex11 Tree Representation and Traversal
## DATE: 13.3.2025
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. Start
2. Define a function display_postorder() that takes a pointer to the root node of the tree.
3. Check if the current node (root_node) is not null.
4. Recursively call display_postorder() for the left child of the current node.
5. Recursively call display_postorder() for the right child of the current node.
6. After visiting both children, print the value of the current node.
7. End 

## Program:
```
/*struct node
{
int value;
struct node*left_child, *right_child;
};*/
void display_postorder(struct node*root_node){
if(root_node)
{
display_postorder(root_node->left_child);
display_postorder(root_node->right_child);
printf("%d\n",root_node->value);
}
}
Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/1cb2df91-25a9-40ab-ad00-764a55d0c6ca)


## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
