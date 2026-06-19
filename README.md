Linked List in C (SLL & DLL)
Task

Implement and compare Singly Linked Lists (SLL) and Doubly Linked Lists (DLL) in C, focusing on insertion, deletion, and pointer handling.

What’s Covered
Add node at end (SLL)
Delete node (SLL vs DLL comparison)
Traversal logic
next and prev pointer handling
Memory allocation with malloc
Key Differences
SLL deletion: requires traversal → O(n)
DLL deletion: uses prev pointer → O(1)
DLL downside: more memory + more complex pointer updates
Common Issues Fixed
Incorrect traversal (stopping at NULL instead of last node)
Missing link updates when inserting nodes
Forgetting malloc NULL checks
Memory leaks from lost node references
Memory Cost (64-bit)
SLL node: ~12 bytes
DLL node: ~20 bytes
Build
gcc *.c -o list
./list
