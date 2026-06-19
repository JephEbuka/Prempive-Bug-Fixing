# 📚 Linked List Implementation in C

## 📌 Task Overview

This project focuses on implementing and understanding **Singly Linked Lists (SLL)** and **Doubly Linked Lists (DLL)** in C. It emphasizes pointer manipulation, dynamic memory allocation, and correct list operations such as insertion and deletion.

---

## 🎯 Objectives

* Implement basic linked list structures in C
* Perform insertion and deletion operations
* Understand pointer behavior in SLL vs DLL
* Identify and fix common memory and logic errors
* Improve debugging skills in low-level C code

---

## 🧱 Data Structures Used

### Singly Linked List (SLL)

```c
typedef struct list_s {
    int n;
    struct list_s *next;
} list_t;
```

### Doubly Linked List (DLL)

```c
typedef struct dlist_s {
    int n;
    struct dlist_s *next;
    struct dlist_s *prev;
} dlist_t;
```

---

## ⚙️ Implemented Operations

* Add node at the end
* Delete a node (SLL & DLL comparison)
* Traversal of list
* Pointer updates (`next` and `prev`)
* Edge case handling (empty list, single node)

---

## ⚠️ Key Learning Points

### 1. SLL vs DLL Deletion

* SLL requires traversal to find previous node → **O(n)**
* DLL uses `prev` pointer → direct access → **O(1)**

---

### 2. Common Bugs Fixed

* Incorrect traversal (stopping at `NULL` instead of last node)
* Not linking new nodes properly
* Missing `malloc` NULL checks
* Memory leaks due to lost node references

---

### 3. Memory Considerations (64-bit system)

* SLL node: `sizeof(int) + sizeof(pointer)` → ~12 bytes
* DLL node: `sizeof(int) + 2 * sizeof(pointer)` → ~20 bytes (excluding padding)

---

## 🧠 Key Insight

DLL improves performance for deletion but increases memory usage and implementation complexity due to dual pointer maintenance.

---

## 🚀 How to Compile

```bash
gcc -Wall -Werror -Wextra -pedantic *.c -o list
./list
```

---

## 📂 Project Structure

```
.
├── sll.c
├── dll.c
├── add_node_end.c
├── delete_node.c
└── README.md
```

---

## 🧪 Author Notes

This project is designed to build strong foundational understanding of pointer-based data structures in C. Focus is not just on working code, but on correctness, safety, and performance trade-offs.
