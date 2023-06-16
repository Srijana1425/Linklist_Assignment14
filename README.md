# Linklist_Assignment14
## 💡 Question 01

> Given a linked list of **N** nodes such that it may contain a loop.
> 
> A loop here means that the last node of the link list is connected to the node at position X(1-based index). If the link list does not have any loop, X=0.
> 
> Remove the loop from the linked list, if it is present, i.e. unlink the last node which is forming the loop.
> 
> **Example 1:**
> ```
> Input:
> N = 3
> value[] = {1,3,4}
> X = 2
> Output:1
> Explanation:The link list looks like
> 1 -> 3 -> 4
>      ^    |
>      |____|
> A loop is present. If you remove it
> successfully, the answer will be 1.
> ```
> 
> **Example 2:**
> ```
> Input:
> N = 4
> value[] = {1,8,3,4}
> X = 0
> Output:1
> Explanation:The Linked list does not
> contains any loop.
> ```
> 
> **Example 3:**
> ```
> Input:
> N = 4
> value[] = {1,2,3,4}
> X = 1
> Output:1
> Explanation:The link list looks like
> 1 -> 2 -> 3 -> 4
> ^              |
> |______________|
> A loop is present.
> If you remove it successfully,
> the answer will be 1.
> ```
> *Answer*<br>
> **Code** [Link]()


## 💡 Question 02

> A number **N** is represented in Linked List such that each digit corresponds to a node in linked list. You need to add 1 to it.
> 
> **Example 1:**
> 
> ```
> Input:
> LinkedList: 4->5->6
> Output:457
> 
> ```
> 
> **Example 2:**
> ```
> Input:
> LinkedList: 1->2->3
> Output:124
> ```
> *Answer*<br>
> **Code** [Link]()

## 💡 Question 03
 
> Given a Linked List of size N, where every node represents a sub-linked-list and contains two pointers:(i) a **next** pointer to the next node,(ii) a **bottom** pointer to a linked list where this node is head.Each of the sub-linked-list is in sorted order.Flatten the Link List such that all the nodes appear in a single level while maintaining the sorted order. **Note:** The flattened list will be printed using the bottom pointer instead of next pointer.
> 
> **Example 1:**
> ```
> Input:
> 5 -> 10 -> 19 -> 28
> |     |     |     |
> 7     20    22   35
> |           |     |
> 8          50    40
> |                 |
> 30               45
> Output: 5-> 7-> 8- > 10 -> 19-> 20->
> 22-> 28-> 30-> 35-> 40-> 45-> 50.
> Explanation:
> The resultant linked lists has every
> node in a single level.(Note:| represents the bottom pointer.)
> ```
> 
> **Example 2:**
> ```
> Input:
> 5 -> 10 -> 19 -> 28
> |          |
> 7          22
> |          |
> 8          50
> |
> 30
> Output: 5->7->8->10->19->22->28->30->50
> Explanation:
> The resultant linked lists has every
> node in a single level.
> 
> (Note:| represents the bottom pointer.)
> ```
> *Answer*<br>
> **Code** [Link]()
## 💡 Question 04

> You are given a special linked list with **N** nodes where each node has a next pointer pointing to its next node. You are also given **M** random pointers, where you will be given **M** number of pairs denoting two nodes **a** and **b**  **i.e. a->arb = b** (arb is pointer to random node)**.**
> 
> Construct a copy of the given list. The copy should consist of exactly **N** new nodes, where each new node has its value set to the value of its corresponding original node. Both the next and random pointer of the new nodes should point to new nodes in the copied list such that the pointers in the original list and copied list represent the same list state. None of the pointers in the new list should point to nodes in the original list.
> 
> For example, if there are two nodes **X** and **Y** in the original list, where **X.arb** **-->** **Y**, then for the corresponding two nodes **x** and **y** in the copied list, **x.arb --> y.**
> 
> Return the head of the copied linked list.
> 
> <img src="https://pwskills.notion.site/image/https%3A%2F%2Fcontribute.geeksforgeeks.org%2Fwp-content%2Fuploads%2Fclone.jpg?id=91feb271-fee1-4199-9997-34833a3388da&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=900&userId=&cache=v2" height="220px">
> 
> **Note** :- The diagram isn't part of any example, it just depicts an example of how the linked list may look like.
> 
> **Example 1:**
> 
> ```
> Input:
> N = 4, M = 2
> value = {1,2,3,4}
> pairs = {{1,2},{2,4}}
> Output:1
> Explanation:In this test case, there
> are 4 nodes in linked list.  Among these
> 4 nodes,  2 nodes have arbitrary pointer
> set, rest two nodes have arbitrary pointer
> as NULL. Second line tells us the value
> of four nodes. The third line gives the
> information about arbitrary pointers.
> The first node arbitrary pointer is set to
> node 2.  The second node arbitrary pointer
> is set to node 4.
> 
> ```
> 
> **Example 2:**
> 
> ```
> Input:
> N = 4, M = 2
> value[] = {1,3,5,9}
> pairs[] = {{1,1},{3,4}}
> Output:1
> Explanation:In the given testcase ,
> applying the method as stated in the
> above example, the output will be 1.
> ```
> *Answer*<br>
> **Code** [Link]()

## 💡 Question 05

> Given the `head` of a singly linked list, group all the nodes with odd indices together followed by the nodes with even indices, and return *the reordered list*.
> 
> The **first** node is considered **odd**, and the **second** node is **even**, and so on.
> 
> Note that the relative order inside both the even and odd groups should remain as it was in the input.
> 
> You must solve the problem in `O(1)` extra space complexity and `O(n)` time complexity.
> 
> **Example 1:**
> 
> <img src="https://pwskills.notion.site/image/https%3A%2F%2Fassets.leetcode.com%2Fuploads%2F2021%2F03%2F10%2Foddeven-linked-list.jpg?id=13e98531-bf7c-461e-ae66-555d769a04ec&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=600&userId=&cache=v2" height="220px">
> 
> ```
> Input: head = [1,2,3,4,5]
> Output: [1,3,5,2,4]
> ```
> 
> **Example 2:**
> 
> <img src="https://pwskills.notion.site/image/https%3A%2F%2Fassets.leetcode.com%2Fuploads%2F2021%2F03%2F10%2Foddeven2-linked-list.jpg?id=d65e07e9-88ca-432c-81bd-06b38ccd8cd4&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=1000&userId=&cache=v2" height="220px">
> 
> ```
> Input: head = [2,1,3,5,6,4,7]
> Output: [2,3,6,7,1,5,4]
> ```
> > *Answer*
> **Code** [Link]()

## 💡 Question 06

> Given a singly linked list of size **N**. The task is to **left-shift** the linked list by **k** nodes, where **k** is a given positive integer smaller than or equal to length of the linked list.
> 
> **Example 1:**
> 
> ```
> Input:
> N = 5
> value[] = {2, 4, 7, 8, 9}
> k = 3
> Output:8 9 2 4 7
> Explanation:Rotate 1:4 -> 7 -> 8 -> 9 -> 2
> Rotate 2: 7 -> 8 -> 9 -> 2 -> 4
> Rotate 3: 8 -> 9 -> 2 -> 4 -> 7
> ```
> 
> **Example 2:**
> ```
> Input:
> N = 8
> value[] = {1, 2, 3, 4, 5, 6, 7, 8}
> k = 4
> Output:5 6 7 8 1 2 3 4
> ```
> *Answer*<br>
> **Code** [Link]()

## 💡 Question 07

> You are given the `head` of a linked list with `n` nodes.
> 
> For each node in the list, find the value of the **next greater node**. That is, for each node, find the value of the first node that is next to it and has a **strictly larger** value than it.
> 
> Return an integer array `answer` where `answer[i]` is the value of the next greater node of the `ith` node (**1-indexed**). If the `ith` node does not have a next greater node, set `answer[i] = 0`.
> 
> **Example 1:**
> 
> <img src="https://pwskills.notion.site/image/https%3A%2F%2Fassets.leetcode.com%2Fuploads%2F2021%2F08%2F05%2Flinkedlistnext1.jpg?id=cae2303b-e908-4f5d-8b20-a4d530752f53&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=610&userId=&cache=v2" height="220px">
> 
> ```
> Input: head = [2,1,5]
> Output: [5,5,0]
> ```
> 
> **Example 2:**
> 
> <img src="https://pwskills.notion.site/image/https%3A%2F%2Fassets.leetcode.com%2Fuploads%2F2021%2F08%2F05%2Flinkedlistnext2.jpg?id=f77103cf-d4e1-4f47-bb0a-247cb26bda15&table=block&spaceId=6fae2e0f-dedc-48e9-bc59-af2654c78209&width=1000&userId=&cache=v2">
> 
> ```
> Input: head = [2,7,4,3,5]
> Output: [7,0,5,5,0]
> ```
> *Answer*<br>
> **Code** [Link]()

## 💡 Question 08

> Given the `head` of a linked list, we repeatedly delete consecutive sequences of nodes that sum to `0` until there are no such sequences.
> 
> After doing so, return the head of the final linked list.  You may return any such answer.
> 
> (Note that in the examples below, all sequences are serializations of `ListNode` objects.)
> 
> **Example 1:**
> 
> ```
> Input: head = [1,2,-3,3,1]
> Output: [3,1]
> Note: The answer [1,2,1] would also be accepted.
> ```
> 
> **Example 2:**
> 
> ```
> Input: head = [1,2,3,-3,4]
> Output: [1,2,4]
> 
> ```
> 
> **Example 3:**
> 
> ```
> Input: head = [1,2,3,-3,-2]
> Output: [1]
> ```
> *Answer*<br>
> **Code** [Link]()
