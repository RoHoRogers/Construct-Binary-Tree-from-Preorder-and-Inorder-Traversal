# Construct-Binary-Tree-from-Preorder-and-Inorder-Traversal
Challenge 105 on leetcode. Decided to use an iterative method

Keep pushing the nodes from the preorder into a stack (and keep making the tree by adding nodes to the left of the previous node) until the top of the stack matches the inorder.

At this point, pop the top of the stack until the top does not equal inorder (keep a flag to note that you have made a pop).

Repeat 1 and 2 until preorder is empty. The key point is that whenever the flag is set, insert a node to the right and reset the flag.
