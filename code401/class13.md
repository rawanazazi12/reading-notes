# What I've Learned at the 13th lecture of 401 code...

## Trees

1. Node - A Tree node is a component which may contain it’s own values, and references to other nodes
2. Root - The root is the node at the beginning of the tree
3. K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
4. Left - A reference to one child node, in a binary tree
5. Right - A reference to the other child node, in a binary tree
6. Edge - The edge in a tree is the link between a parent and child node
7. Leaf - A leaf is a node that does not have any children
8. Height - The height of a tree is the number of edges from the root to the furthest leaf

9. Sample Tree
 
 ![simple tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)


10. Traversals        
   An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

   - Depth First
   - Breadth First

11. Depth First
    Depth first traversal is where we prioritize going through the depth (height) of the tree first.
    - Pre-order: root >> left >> right
    - In-order: left >> root >> right
    - Post-order: left >> right >> root


12. Breadth First
    Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.