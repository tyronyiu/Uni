---
layout: post
title: "Depth-First vs Breadth-First Search "
date: 2019-01-28
author: "Kevin Ko"
categories: Code Tech Algorithms
---


If you’ve taken the time to study code in any shape or form, you’ve probably
come across data structures. Data structures are comprised of a plethora of
possibilities for storing, organizing, and manipulating data. Some of the more
popular ones include arrays, linked lists, stacks, queues, and binary search
trees. For the sake of this article, we’ll be focusing on two different ways to
approach tree traversal: Depth-First Search and Breadth-First Search.

#### **What is a tree?**

A tree is a data structure comprised of nodes, which contain pointers to other
nodes. Unlike trees in real life (or maybe they exist somewhere), a data tree is
upside-down. Essentially, the root is at the top and the leaves are at the
bottom.

![](https://cdn-images-1.medium.com/max/1600/0*vR1ynYt4DKHqct5m.jpg)

Let’s break down the diagram.

Every tree has a single root node which is at the top level (in this case, level
0). Then we see that at the next level, the root node A has pointers to nodes B
and C. Likewise, nodes B and C have pointers to node A. In this situation, node
A is the parent node, and nodes B and C are its children. Furthermore, nodes B
and C are considered siblings.

*You may be wondering if it is possible for a node to have more than 2 children.
The answer is yes! This specific depiction is of a binary tree which can be
determined by a maximum of two child nodes for each parent.*

**Tree Code**

*Disclaimer: I will be using Javascript to create a simple tree!*

Firstly, we need to create a node class:

When we create a node class we pass it a value, or data, which becomes the data
property of the node. We also have parent and children properties which are null
and an empty array, respectively, for now. Eventually, the parent property will
point to the parent of the specific node and the children property will point to
the node’s children.

Then, we create the tree class:

The tree class contains a single property, root, that is initially null. Trees
include prototype methods such as contains(), insert(), and remove(), but we’ll
save those for a rainy day!

#### Searching!

Both depth-first and breadth-first searches are prototype methods of the Tree
class which are used to determine whether a particular node containing specific
data exists within a tree. The depiction below shows the two different searching
procedures.

#### **Depth-First Approach**

The depth-first method starts at the root node and moves towards the left-most
node. Once it hits the left-most node, it traverses up the tree back to the root
and then to the right-most node. If it hits a node with children, it will
traverse through that node’s children from left to right and then continue
rightwards.

Search Order: [10, 4, 1, 9, 17, 12, 18]

**Code**

Depth-first search takes in a value as an argument which is the value we’re
looking for in the tree. Since we want to traverse the nodes from left to right,
we set the root as a stack because we want to take a last in first out approach.
Then we perform a while loop which continues as long as the stack contains
elements. Within the while loop, we remove the first element in the stack, or
call the shift() array method, and set it equal to a node. We compare that
node’s data to the argument value and if they match, the function returns true.
If this is not the case, it adds the node’s children to the front of the stack,
or calls the unshift() array method, and continues searching through the new
data. If the particular value does not exist in the tree, the function returns
false.

#### **Breadth-First Approach**

The breadth-first approach starts at the root node and traverses through each
successive level to search for the desired node. Similarly to the depth-first
approach, the nodes are read from left to right at each level.

Search Order: [10, 4, 17, 1, 9, 12, 18]

**Code**

Breadth-first search is similar in code to depth-first search. It takes in a
value to be found as an argument. The difference here is that instead of
utilizing a stack, we want to use a queue to be able to take a first in first
out approach. In the while loop, similarly to depth-first search, we want to use
the shift() array method to remove the first element of the queue as a node.
However, if the node data is not the same as the value desired, instead of
unshifting the node’s children, we will use the push() array method to add the
children to the end of the queue. This allows us to check the every node in a
level before traversing through the nodes in the next level. Finally, just like
depth-first search, if the value isn’t found, the function will return false.

#### Which Do I Use?

Though both depth-first(DFS) and breadth-first(BFS) searches are legitimate
approaches and can reach the same conclusions, each one is favored under certain
circumstances. However, it is not often obvious which one is more efficient of
the two.

*Disclaimer: These are general guidelines! Definitely not always the most
optimal approaches.*

DFS: Generally preferred when the tree is very deep and desired values or data
occurs infrequently.

BFS: Generally preferred in shallow trees that aren’t too wide. Also used if it
is known that the desired node is closer to the root level.

Even though there are general preferences when deciding which method to utilize,
if you are unsure, it is probably better to try both methods and see which one
is more efficient.

For example, let’s say you’re using the tree above and you’re looking for the
node containing 8. The tree isn’t that deep so you might think it would be
better to utilize a BFS. However, it would actually be more efficient to use a
DFS.

Let’s compare the two methods and which nodes have been traversed:

DFS: 1, 2, 4, 8

BFS: 1, 2, 3, 4, 5, 6, 7, 8

Already we can see that a breadth-first search traverses through more nodes and
therefore needs access to more memory.

Furthermore, once we locate node 8, the DFS stack would be [8, 9, 5, 3] while
the BFS queue would be [8, 9, 10, 11, 13, 14]. The BFS queue contains 2 more
nodes, which doesn’t seem to equate to much in this example, but in terms of
memory, it still uses a greater amount. Therefore, in this particular situation,
a DFS would be more efficient than a BFS.

Though this example is simple and straightforward, in situations where trees are
deeper and wider, it is definitely much more difficult to determine which is
more optimal. The best way to dictate the better method is to attempt both.

### Complexity

Time and space complexity for both DFS and BFS are pretty straightforward. Since
we’re speaking of tree traversal, in order to determine if a value or data
exists within the tree, we must visit every node. Visiting every node a single
time means that the time complexity for both DFS and BFS are O(n), or linear. If
we think about trees as sorted arrays, we would only have to lop through a
single time to determine whether or not a value matches the value we’re
searching for. Similarly, in terms of space complexity, DFS is O(h) and BFS is
O(w). For DFS, ‘h’ stands for height since how much space the function will take
depends on how many nodes deep the tree is. Likewise, for BFS, ‘w’ stands for
width, since space depends on how wide the tree is. Of course, these big O
notations change depending on the data structure, but for the sake of trees, the
time and space complexities will be the same.

*****

Thank you for taking the time to read this article! If you have any feedback or
questions, let me know! Hope you have a great day!

* [Programming](https://medium.com/tag/programming?source=post)
* [JavaScript](https://medium.com/tag/javascript?source=post)

### [Kevin Ko](https://medium.com/@kevin.hw.ko)
