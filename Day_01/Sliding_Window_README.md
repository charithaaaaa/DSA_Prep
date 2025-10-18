# 💻 Sliding Window DSA Practice – 20 Essential Problems

## 🚀 Day 1 of DSA Preparation

This repository tracks my progress in mastering the **Sliding Window Technique** in Data Structures and Algorithms (DSA). This technique is crucial for optimizing problems involving **subarrays or substrings** to achieve an efficient $O(n)$ time complexity.

---

## 📘 Sliding Window Overview 🪟

The core idea is to "slide" a window (defined by two pointers) across an array or string, reusing calculations from the previous step to avoid redundant computations.

| Feature | Description | Complexity |
| :--- | :--- | :--- |
| **Time Complexity** | $O(n)$ — Each element enters and leaves the window once. |
| **Space Complexity** | $O(k)$ or $O(1)$, depending on data structures used (e.g., hash map, deque). |

---

## 🧩 Types of Sliding Windows

### 1. **Fixed-size Sliding Window**
Used when the window length **$k$ is constant**.
* **Mechanism:** Keep track of a running metric (e.g., sum) and update it by subtracting the element leaving the window and adding the element entering it.

### 2. **Variable-size Sliding Window**
Used to find the **longest/shortest** subarray/substring that satisfies a **specific condition**.
* **Mechanism:** Use two pointers (`left`, `right`). Expand with `right`. When the window violates the condition, contract with `left` until the condition is met again.

### 3. **Monotonic Deque-based Sliding Window**
Used to efficiently track the **maximum/minimum** element within the current window in $O(1)$ time.
* **Mechanism:** A `Deque` maintains indices of elements in a strictly **monotonic** (increasing or decreasing) order of their values.

---

## 🔥 20 Essential Practice Problems

### 🧊 Fixed Size Sliding Window (Focus for Day 1)
These problems involve a constant window size $k$.

| # | Problem | Source & Link | Key Tool |
| :---: | :--- | :--- | :--- |
| 1 | **Maximum Sum Subarray of Size K** | [GFG](https://www.geeksforgeeks.org/problems/max-sum-subarray-of-size-k5313/1) | Running sum |
| 2 | **Maximum Average Subarray I** | [LeetCode 643](https://leetcode.com/problems/maximum-average-subarray-i/) | Running sum |
| 3 | **Maximum Sum Circular Subarray** | [LeetCode 918](https://leetcode.com/problems/maximum-sum-circular-subarray/) | Fixed Window Logic + Kadane's |
| 4 | **Count Occurrences of Anagrams** | [GFG](https://www.geeksforgeeks.org/problems/count-occurences-of-anagrams5839/1) | Frequency Map |
| 5 | **Find All Anagrams in a String** | [LeetCode 438](https://leetcode.com/problems/find-all-anagrams-in-a-string/) | Frequency Map |

---

### 🔄 Variable Size Sliding Window
These problems involve dynamic window adjustment.

| # | Problem | Source & Link | Key Tool |
| :---: | :--- | :--- | :--- |
| 6 | **Longest Substring Without Repeating Characters** | [LeetCode 3](https://leetcode.com/problems/longest-substring-without-repeating-characters/) | Hash Set or Map |
| 7 | **Longest Substring with At Most K Distinct Characters** | [LeetCode 340](https://leetcode.com/problems/longest-substring-with-at-most-k-distinct-characters/) | Frequency Map |
| 8 | **Fruit Into Baskets (Max two unique types)** | [LeetCode 904](https://leetcode.com/problems/fruit-into-baskets/) | Frequency Map (K=2) |
| 9 | **Longest K Unique Characters Substring** | [GFG](https://www.geeksforgeeks.org/problems/longest-k-unique-characters-substring0853/1) | Frequency Map |
| 10 | **Subarrays with K Different Integers** | [LeetCode 992](https://leetcode.com/problems/subarrays-with-k-different-integers/) | "At Most K" Template |

---

### 📉 Monotonic Deque / Max-Min in Window
These utilize a Deque for efficient extremum tracking.

| # | Problem | Source & Link | Key Tool |
| :---: | :--- | :--- | :--- |
| 11 | **Sliding Window Maximum** | [LeetCode 239](https://leetcode.com/problems/sliding-window-maximum/) | Monotonic Deque (Decreasing) |
| 12 | **First Negative Integer in Every Window of Size K** | [GFG](https://www.geeksforgeeks.org/problems/first-negative-integer-in-every-window-of-size-k3345/1) | Queue or Deque |
| 13 | **Sum of Minimum and Maximum Elements of All Subarrays of Size K** | [GFG](https://www.geeksforgeeks.org/problems/sum-of-minimum-and-maximum-elements-of-all-subarrays-of-size-k/0) | Two Monotonic Deques (Max and Min) |

---

### 📊 Counting & Sum Patterns
These problems often involve counting valid subarrays or finding the minimum-sized window.

| # | Problem | Source & Link | Key Tool |
| :---: | :--- | :--- | :--- |
| 14 | **Subarray Product Less Than K** | [LeetCode 713](https://leetcode.com/problems/subarray-product-less-than-k/) | Running Product, Variable Window |
| 15 | **Minimum Window Substring** | [LeetCode 76](https://leetcode.com/problems/minimum-window-substring/) | Frequency Map (Hardest) |
| 16 | **Smallest Subarray with Sum Greater Than X** | [GFG](https://www.geeksforgeeks.org/problems/smallest-subarray-with-sum-greater-than-x5651/1) | Running Sum, Variable Window |
| 17 | **Longest Subarray with Sum K** | [GFG](https://www.geeksforgeeks.org/problems/longest-sub-array-with-sum-k0809/1) | Running Sum + Hash Map (Prefix Sum Hybrid) |

---

### 🎯 Harder Variants / Transformation
These problems combine Sliding Window with other concepts (like bit manipulation or max frequency count).

| # | Problem | Source & Link | Key Tool |
| :---: | :--- | :--- | :--- |
| 18 | **Max Consecutive Ones III** | [LeetCode 1004](https://leetcode.com/problems/max-consecutive-ones-iii/) | Count of Zeros, Variable Window |
| 19 | **Longest Repeating Character Replacement** | [LeetCode 424](https://leetcode.com/problems/longest-repeating-character-replacement/) | Frequency Map, Max Frequency |
| 20 | **Binary Subarrays With Sum** | [LeetCode 930](https://leetcode.com/problems/binary-subarrays-with-sum/) | "At Most K" Template |
