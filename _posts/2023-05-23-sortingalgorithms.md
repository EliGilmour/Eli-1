---
toc: true
layout: post
Badges: true
comments: false
author: Eli gilmour
categories: [fastpages, markdown]
title: Sorting Algorithms Hacks
---

# 1

- Primitive types in Python include fundamental data types such as integers, floating-point numbers, strings, booleans, and None. These types represent basic values and have a fixed size in memory.

- Python doesn't have explicit pass-by-reference semantics, the behavior of passing a list to a function resembles pass-by-reference, as modifications to the list within the function persist after the function call.

# Practice Problems

1. Bubble sort is a simple sorting algorithm that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. This process is repeated until the entire list is sorted.
    Selection sort is another simple sorting algorithm that works by dividing the list into a sorted and an unsorted region. It repeatedly finds the smallest (or largest) element from the unsorted region and swaps it with the leftmost unsorted element, expanding the sorted region by one element.

2. Merge sort is a divide-and-conquer algorithm that recursively divides the list into smaller sublists, sorts them, and then merges them back together to obtain a sorted list. It has a time complexity of O(n log n).
    insortion sort, It iterates through the list and repeatedly inserts each element into its correct position within the already sorted part of the list. It has a time complexity of O(n^2).

# What happened to this sort

- Its comparing the twoo block and seeing which one is higher and lower and switching to be in the right order. Then it continues through the whole list to make sure the whole list is sorted.

# Stargies to sort this code ( Warmup )

- Bubble Sort: Iterate through the list multiple times, comparing adjacent elements and swapping them if they are in the wrong order. This process is repeated until the list is sorted.

Selection Sort: Find the minimum element in the unsorted part of the list and swap it with the first unsorted element. Repeat this process for the remaining unsorted part until the entire list is sorted.