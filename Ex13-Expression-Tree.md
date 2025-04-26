# Ex13 Expression Tree
## DATE: 17.3.2025
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1.Start the program.

2.For preorder, print the node data, then recursively traverse the left and right subtrees.

3.For inorder, recursively traverse the left subtree, print the node data, then traverse the right subtree.

4.For postorder, recursively traverse the left and right subtrees, then print the node data.

5.Use recursive functions handling each node via tree->d (data), tree->l (left), and tree->r (right).



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

Developed by:  DHARSHINIYAA KS
RegisterNumber:  212223100004

```

## Output:

![image](https://github.com/user-attachments/assets/88db3995-7cb8-4647-b3b2-c6ade183d9d4)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
