# Trees

---

# Common trees terminologies

| term   | meaning                                                                                                           |
| ------ | ----------------------------------------------------------------------------------------------------------------- |
| Node   | A Tree node is a component which may contain it’s own values, and references to other nodes                       |
| Root   | The root is the node at the beginning of the tree                                                                 |
| K      | A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2 |
| Left   | A reference to one child node, in a binary tree                                                                   |
| Right  | A reference to the other child node, in a binary tree                                                             |
| Edge   | The edge in a tree is the link between a parent and child node                                                    |
| Leaf   | A leaf is a node that does not have any children                                                                  |
| Height | The height of a tree is the number of edges from the root to the furthest leaf                                    |

![sample tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

---

## Traversals

There are two categories of traversals:

1. Depth First.
2. Breadth First.

**Depth First**

- Depth first traversal is where we prioritize going through the depth (height) of the tree first.

- three methods for depth first traversal:

1. Pre-order: `root >> left >> right`
2. In-order: `left >> root >> right`
3. Post-order: `left >> right >> root`

**Breadth First**

- Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.
- breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree.

---

## Binary Tree Vs K-ary Trees

| Binary Tree                                                                                                                                                               | K-ary Trees                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Binary Trees restrict the number of children to two and there is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows | If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have. |

---

## Big O

- The Big O time complexity for inserting a new node is O(n).
- Searching for a specific node will also be O(n) ❓ Why ❓
- The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree.
- A “perfect” binary tree is one where every non-leaf node has exactly two children. The maximum width for a perfect binary tree, is 2^(h-1), where h is the height of the tree.

![tree](https://miro.medium.com/max/975/1*PWJiwTxRdQy8A_Y0hAv5Eg.png)
