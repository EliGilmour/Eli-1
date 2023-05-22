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

my_list = [
    {"name": "Alice", "age": 25, "city": "London"},
    {"name": "Bob", "age": 32, "city": "New York"},
    {"name": "Charlie", "age": 19, "city": "Paris"},
    {"name": "David", "age": 41, "city": "Tokyo"},
    {"name": "Eve", "age": 28, "city": "Berlin"}
]

# Display the original list

print("Original List:")
print(my_list)

# Testing bubble sort on your list

print("\nBubble Sort:")
start_time = time.time()
for key in my_list[0]:
    bubbleSort(my_list, key)
    print(f"\nSorted by '{key}':")
    print(my_list)
end_time = time.time()
bubble_sort_time = end_time - start_time

# Testing merge sort on your list

print("\nMerge Sort:")
start_time = time.time()
for key in my_list[0]:
    mergeSort(my_list, key)
    print(f"\nSorted by '{key}':")
    print(my_list)
end_time = time.time()
merge_sort_time = end_time - start_time

# Analysis of sorting algorithms

print("\nSorting Analysis:")
print(f"Number of elements: {len(my_list)}")
print(f"Bubble Sort Comparisons: {len(my_list) * (len(my_list) - 1) // 2}")
print(f"Bubble Sort Swaps: {len(my_list) * (len(my_list) - 1) // 2}")
print(f"Bubble Sort Time: {bubble_sort_time} seconds")
print(f"Merge Sort Comparisons: {len(my_list) * (len(my_list) - 1) // 2}")
print(f"Merge Sort Swaps: {len(my_list) * (len(my_list) - 1) // 2}")
print(f"Merge Sort Time: {merge_sort_time} seconds")
