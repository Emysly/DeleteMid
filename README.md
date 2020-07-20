# DeleteMid
## A program to delete a node from the middle of the singly linked list

In this program, we will create a singly linked list and delete a node from the middle of the list. To accomplish this task, we will calculate the size of the list and then divide it by 2 to get the mid-point of the list. Node temp will point to head node. We will iterate through the list till midpoint is reached. Now, the temp will point to middle node and node current will point to node previous to temp. We delete the middle node such that current's next node will point to temp's next node.

![](https://static.javatpoint.com/corebasic/programs/images/java-program-to-delete-a-node-from-the-middle-of-the-singly-linked-list.png)

Java program to delete a node from the middle of the singly linked list
Consider the above example, mid-point of the above list is 2. Iterate temp from head to mid-point. Now, temp is pointing to the mid node which needs to be deleted. In this case, Node is the middle node which needs to be deleted. The node can be deleted by making node 2's next (current) to point to node 3 (temp's next node). Set temp to null.

Algorithm
Create a class Node which has two attributes: data and next. Next is a pointer to the next node in the list.
Create another class deleteMid which has three attributes: head, tail, and size which keep tracks of the number of nodes present in the list.
addNode() will add a new node to the list:
Create a new node.
It first checks, whether the head is equal to null which means the list is empty.
If the list is empty, both head and tail will point to the newly added node.
If the list is not empty, the new node will be added to end of the list such that tail's next will point to the newly added node. This new node will become the new tail of the list.
a. deleteFromMid() will delete a node from the middle of the list:


It first checks whether the head is null (empty list) then, display the message "List is empty" and return.
If the list is not empty, it will check whether the list has only one node.
If the list has only one node, it will set both head and tail to null.
If the list has more than one node then, calculate the size of the list and divide it by 2 to get the mid-point of the list.
Declare a node temp which will point to head and node current will point to node previous to temp.
Traverse through the list till temp points to a middle node. If current not point to null then, delete the middle node(temp) by making current's next to point to temp's next. Else, both head and tail will point to node next to temp and delete the middle node by setting the temp to null.
a. display() will display the nodes present in the list:

Define a node current which will initially point to the head of the list.
Traverse through the list till current points to null.
Display each node by making current to point to node next to it in each iteration.
