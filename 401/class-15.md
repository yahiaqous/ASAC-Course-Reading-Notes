# Trees

## Common Terminology

- **Node** - A Tree node is a component that may contain its own values, and references to other nodes

- **Root** - The root is the node at the beginning of the tree

- **K** - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

- **Left** - A reference to one child node, in a binary tree

- **Right** - A reference to the other child node, in a binary tree

- **Edge** - The edge in a tree is the link between a parent and child node

- **Leaf** - A leaf is a node that does not have any children

- **Height** - The height of a tree is the number of edges from the root to the furthest leaf

![BinaryTree](./Pictures/BinaryTree1.png)

## Traversals

There are two categories of traversals when it comes to trees:

1. **Depth First**: Depth-first traversal is where we prioritize going through the depth (height) of the tree first.

- **Pre-order** - root >> left >> right "the root has to be looked at first"
- **In-order** - left >> root >> right
- **Post-order** - left >> right >> root

  2.**Breadth First**: Breadth-first traversal iterates through the tree by going through each level of the tree node-by-node.
