# binary-tree #
A doubly-linked binary tree (with a pointer to `left`, `right` and `prev`).

## How to use direction strings ##

When using certain functions, such as `tree_seek`, it is necessary to provide
a direction string. For example, consider the following binary tree:

(`B_NODE_T` has been set to	`float`, and the head of the tree is `head`)
```
                  "ll": 1.1
                 /
         "l": 1.0
        /        \ 
 "": 0.0          "lr": 1.2
        \
         \          "rl": 2.1
          \        /
           "r": 2.0
                   \
                    "rr": 2.2
```
The strings at each node show the required direction string. (The colons are
not part of the direction string.)

For example,`tree_seek(head, "")` returns a pointer to the head of the
tree.
