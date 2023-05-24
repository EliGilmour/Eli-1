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






# Merge sorts a list of dictionaries based on provided key
def mergeSort(arr, key):
    if len(arr) > 1:
        mid = len(arr) // 2
        left_half = arr[:mid]
        right_half = arr[mid:]

        mergeSort(left_half, key)
        mergeSort(right_half, key)

        i = j = k = 0

        while i < len(left_half) and j < len(right_half):
            if left_half[i].get(key) < right_half[j].get(key):
                arr[k] = left_half[i]
                i += 1
            else:
                arr[k] = right_half[j]
                j += 1
            k += 1

        while i < len(left_half):
            arr[k] = left_half[i]
            i += 1
            k += 1

        while j < len(right_half):
            arr[k] = right_half[j]
            j += 1
            k += 1

# Create your own list

Eli_list = [
    {"name": "Bob", "age": 25, "city": "London"},
    {"name": "Khalid", "age": 32, "city": "New York"},
    {"name": "Eli", "age": 19, "city": "Paris"},
    {"name": "David", "age": 41, "city": "Tokyo"},
    {"name": "Eve", "age": 28, "city": "Berlin"}
]

# Display the original list

print("Original List:")
print(Eli_list)

# Testing bubble sort on your list

print("\nBubble Sort:")
start_time = time.time()
for key in Eli_list[0]:
    bubbleSort(Eli_list, key)
    print(f"\nSorted by '{key}':")
    print(Eli_list)
end_time = time.time()
bubble_sort_time = end_time - start_time

# Testing merge sort on your list

print("\nMerge Sort:")
start_time = time.time()
for key in my_list[0]:
    mergeSort(Eli_list, key)
    print(f"\nSorted by '{key}':")
    print(Eli_list)
end_time = time.time()
merge_sort_time = end_time - start_time

# Analysis of sorting algorithms

print("\nSorting Analysis:")
print(f"Number of elements: {len(Eli_list)}")
print(f"Bubble Sort Comparisons: {len(Eli_list) * (len(Eli_list) - 1) // 2}")
print(f"Bubble Sort Swaps: {len(Eli_list) * (len(Eli_list) - 1) // 2}")
print(f"Bubble Sort Time: {bubble_sort_time} seconds")
print(f"Merge Sort Comparisons: {len(Eli_list) * (len(Eli_list) - 1) // 2}")
print(f"Merge Sort Swaps: {len(Eli_list) * (len(Eli_list) - 1) // 2}")
print(f"Merge Sort Time: {merge_sort_time} seconds")

# Bubble Sort Poopcorn Hack

words = new_words()
print(words)
def bubbleSort(list):
    n = len(list) - 1  # list are indexed 0 to n-1, len is n
    
    # Traverse through list with i index
    for i in range(n):
        swapped = False  # optimize code, so it exits if now swaps on inner loop

        # Inner traversal using j index
        for j in range(n-i):  # n-i as positions on right are in order in bubble
 
            # Swap if the element KeyN is greater KeyN1
            keyN = list[j]
            keyN1 = list[j+1]
            if keyN > keyN1:
                swapped = True
                list[j], list[j + 1] = list[j + 1], list[j]  # single line swap
         
        if not swapped:  # if no swaps on inner pass, list is sorted
            return  # exit function
        
bubbleSort(words)
print(words)

# Selection Sort Poopcorn Hack

words = new_words()
print(words)
def selectionSort(list):
    n = len(list)  # length is n
    
    # List is traversed from index 0 to n-1, n elements
    for i in range(n):
        smallI = i  # small index is captured
        smallV = list[i]

        # Inner traversal looks at elements after i
        for j in range(i+1, n):
            # Save reference if less
            keyV = list[j]
            if keyV < smallV:
                smallI = j  # small index is replaced
                smallV = keyV
        
        # swap smallest to current i positon, sorting left to right
        list[i], list[smallI] = list[smallI], list[i]  # single line swap 
        
selectionSort(words)
print(words)