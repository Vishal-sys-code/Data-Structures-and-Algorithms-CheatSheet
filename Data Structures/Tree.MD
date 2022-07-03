# Tree

![Tree](/images/tree.png)

A tree whose elements have at most 2 children is called a binary tree. Since each element in a binary tree can have only 2 children, we typically name them the left and right child.

<br>

A Binary Tree node contains the following parts:

* Data.
* Pointer to left child.
* Pointer to right child.

A tree is a popular data structure that is non-linear in nature.

* **Root**: The root of a tree is the topmost node of the tree that has no parent node. There is only one root node in every tree.
* **Edge**: Edge acts as a link between the parent node and the child node.
* **Leaf**: A node that has no child is known as the leaf node. It is the last node of the tree. There can be multiple leaf nodes in a tree.
* **Depth**: The depth of the node is the distance from the root node to that particular node.
* **Height**: The height of the node is the distance from that node to the deepest node of the tree.
* **Height of tree**: The Height of the tree is the maximum height of any node.

```
      tree
      —-
         j    <– root
        / \
       /   \
      f      k  
     / \      \
    a  h       z    <– leaves
```