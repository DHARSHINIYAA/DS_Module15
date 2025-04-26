# Ex14 Heap Tree
## DATE: 17.3.2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm:
1.Start the program.

2.Use recursion to handle each node with tree->d (data), tree->l (left), and tree->r (right).

3.In preorder, print node data first, then traverse left and right subtrees.

4.In inorder, traverse left subtree, print node data, then traverse right subtree.

5.In postorder, traverse left and right subtrees first, then print node data.

6.End the program.


## Program:
```
struct n {
char d;
struct n*l;
struct n*r;
};*/
void preOrder(struct n*tree)
{
if(tree)
{
printf("%c",tree->d);
preOrder(tree->l);
preOrder(tree->r);
}
}
void inOrder(struct n*tree)
{
if(tree)
{
inOrder(tree->l);
printf("%c",tree->d);
inOrder(tree->r);
}
}
void postOrder(struct n*tree)
{
if(tree)
{
postOrder(tree->l);
postOrder(tree->r);
printf("%c",tree->d);
}
}

Developed by: DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/0e0d4d3d-b04b-492d-b99d-2c599b11e8a8)


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
