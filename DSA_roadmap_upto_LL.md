# 🗺️ DSA Roadmap with JavaScript (Up to Linked Lists Only)

> **Goal**: Land a job with strong DSA fundamentals in JavaScript  
> **Scope**: Covers **Arrays, Strings, Searching, Sorting, Hash Tables, Recursion, Stacks, Queues, Linked Lists**  
> **Excludes**: Trees, Graphs, Heaps, Tries, Advanced DP, Segment Trees, etc.  
> **Difficulty Cap**: Easy to Medium (LeetCode-style), no advanced data structures beyond Linked Lists.

---

## ✅ Phase 1: Complexity Analysis (1–2 Days)
- **Big O Notation**: 
  - `O(1)`, `O(log n)`, `O(n)`, `O(n log n)`, `O(n²)`
  - Time vs. Space trade-offs
- **How to Analyze**:
  - Loops, nested loops, recursion depth
  - Built-in methods: `sort()` = O(n log n), `includes()` = O(n), `Map.get()` = O(1) avg
- **Practice**: Always state time/space complexity before coding.

---

## ✅ Phase 2: Core Topics (In Order)

### 🔹 1. Arrays & Strings (5–7 Days)
- **Key Patterns**:
  - Two Pointers (same/opposite direction)
  - Sliding Window
  - In-place modification
  - Frequency counting
- **Must-Know Problems**:
  - Two Sum
  - Valid Anagram
  - Reverse String
  - Remove Duplicates from Sorted Array
  - Rotate Array
  - Move Zeroes
  - Valid Palindrome

---

### 🔹 2. Searching Algorithms (2–3 Days)
> All based on **arrays/strings** — no trees needed.

- **Linear Search**: O(n) — trivial but foundational.
- **Binary Search**: **Critical!** (O(log n))
  - Works only on **sorted arrays**
  - Template: `left`, `right`, `mid`
  - Variants: find first/last occurrence, search in rotated array (medium)
- **Must-Know Problems**:
  - Binary Search (classic)
  - Find First and Last Position of Element in Sorted Array
  - Search Insert Position
  - Find Smallest Letter Greater Than Target
  - **Medium (allowed)**: Search in Rotated Sorted Array *(uses binary search logic, no trees)*

> 💡 **Note**: Binary search is **very common** in interviews — master it!

---

### 🔹 3. Sorting Algorithms (3–4 Days)
> Focus on **concepts + usage**, not full manual implementation (unless asked).

- **Built-in Sort**: `arr.sort((a, b) => a - b)` → O(n log n)
- **Understand These** (concept + when to use):
  - **Merge Sort**: Stable, O(n log n), divide & conquer → useful for linked lists!
  - **Quick Sort**: Avg O(n log n), worst O(n²), in-place
  - **Bubble/Insertion/Selection**: O(n²) — know for interviews, rarely used
- **Custom Sorting**:
  - Sort by frequency, length, custom rules (e.g., "sort by last digit")
- **Must-Know Problems**:
  - Sort an Array (implement merge/quick sort if asked)
  - Valid Anagram (via sorting)
  - Meeting Rooms (sort by start time)
  - Height Checker (compare with sorted version)
  - **Linked List Bonus**: Sort List (merge sort on linked list — **highly recommended!**)

> ✅ **Important**: You **must** know how to **sort arrays of objects** and **apply sorting to solve problems**.

---

### 🔹 4. Hash Tables (Objects & Maps) (3–4 Days)
- **Key Concepts**:
  - Hashing, collisions (conceptual)
  - `Map` vs `Object` in JS
- **Must-Know Problems**:
  - Two Sum (again, with hash map)
  - Group Anagrams
  - Subarray Sum Equals K
  - First Unique Character in a String
  - Intersection of Two Arrays II

---

### 🔹 5. Recursion (3–4 Days)
- **Key Concepts**:
  - Base case, recursive case, call stack
  - Convert iterative → recursive (and vice versa)
- **Must-Know Problems**:
  - Fibonacci
  - Power (x^n)
  - Reverse String (recursively)
  - Sum of Array
  - **Bonus**: Merge Two Sorted Lists (recursive approach)

---

### 🔹 6. Stacks & Queues (4–5 Days)
- **Implement using JS arrays**:
  - Stack: `push()` / `pop()`
  - Queue: `push()` / `shift()` (or use index pointer for efficiency)
- **Must-Know Problems**:
  - Valid Parentheses
  - Implement Queue using Stacks
  - Daily Temperatures (monotonic stack)
  - Design Circular Queue (use array + pointers)

---

### 🔹 7. Linked Lists (7–10 Days)
- **Node Structure**:
  ```javascript
  class ListNode {
    constructor(val, next = null) {
      this.val = val;
      this.next = next;
    }
  }
