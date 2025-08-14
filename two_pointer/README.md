# Mastering Two Pointers: The Secret Sauce Behind Pair, Triplet, and Quad Sum Problems

Welcome to your very first PrepLetter! Today, we’re diving into a technique that’s a true interview favorite: the **Two Pointers** pattern. If you’re prepping for technical interviews, you’ll encounter this strategy everywhere from arrays to strings, from pairs to quadruplets.

## What is the Two Pointers Technique?

The **Two Pointers** technique involves using two indices (pointers) that move through the data structure (usually an array) in a coordinated way. Typically, you’ll set one pointer at the start and another at the end, moving them towards each other depending on the problem’s requirements.

### Why Use Two Pointers?

- **Efficiency**: It can reduce your algorithm from O(n^2) to O(n) or O(n^2) from O(n^3).
- **Ideal For**: Sorted arrays and problems involving sums, subarrays, or searching for relationships between elements.

### Simple Example

Suppose you have a sorted array: `[1, 2, 4, 7, 11, 15]` and you want to find if any two numbers sum to 15.
- Start with left pointer `l = 0` and right pointer `r = 5` (the ends).
- Check `arr[l] + arr[r]`. If it’s less than 15, move `l` right. If it’s more, move `r` left. If equal, you found the pair!

This approach is the backbone for a family of popular LeetCode problems: **Two Sum**, **3Sum**, and **4Sum**. Each increases in complexity, but the heart of the solution remains the same: fix some numbers and use two pointers to find the rest.

### Let’s level up, step by step.

## Problem 1: Two Sum II – Input Array Is Sorted

### Two Sum II – LeetCode #167

#### Problem Statement (In Plain English)

Given a sorted array of integers and a target value, find the indices (1-based) of two numbers that add up to the target. Assume exactly one solution exists, and you cannot use the same element twice.

### Example:
**Input**: 
```plaintext
numbers = [2, 7, 11, 15], target = 9
**Output**:
[1, 2]
Explanation:
2 + 7 = 9, and those are at indices 1 and 2 (1-based).
Another Example (Try This Yourself!)
numbers = [1, 3, 4, 6, 8, 10], target = 14
What should the output be? Grab a pen and paper before reading on!
Pause and Solve

Take a moment to try solving this on your own before reading the solution.
Time Complexity:

O(n) where n is the number of elements in the array. We are only iterating through the array once.

Space Complexity:

O(1) because no extra space is used except for the two pointers.
