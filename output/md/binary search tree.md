---
date: 2023-03-18
draft: true
sr-due: 2024-01-02
sr-ease: 270
sr-interval: 230
tags:
- inbox
- definition
---

# Binary search tree

> In [computer science](./binary%20search%20tree.md), a binary search tree
> (BST), also called an ordered or sorted binary tree, is a rooted binary tree
> data structure with the key of each internal node being greater than all the
> keys in the respective node's left subtree and less than the ones in its right
> subtree. The time complexity of operations on the binary search tree is
> directly proportional to the height of the tree.
>
> -- [Wikipedia](https://en.wikipedia.org/wiki/Binary_search_tree)

A binary search tree is a binary tree data structure that works based on the
principle of [binary search](./binary%20search%20algorithm.md).

|           |             |                |
| --------- | ----------- | -------------- |
| Algorithm | **Average** | **Worst case** |
| Space     | O(_n_)      | O(_n_)         |
| Search    | O(log _n_)  | O(_n_)         |
| Insert    | O(log _n_)  | O(_n_)         |
| Delete    | O(log _n_)  | O(_n_)         |