# Algorithms

| Category               | Algorithms                                              |
|------------------------|---------------------------------------------------------|
| Sorting Algorithms     | 1. Bubble Sort ⏬ 🔗<br>2. Selection Sort ⏬ 🔗<br>3. Insertion Sort ⏬ 🔗<br>4. Merge Sort ⏬ 🔗<br>5. QuickSort ⏬ 🔗<br>6. Heapify and Heap Sort ⏬ 🔗<br>7. Counting Sort ⏬ 🔗<br>8. Radix Sort ⏬ 🔗 |
| Searching Algorithms   | 1. Linear Search ⏬ 🔗<br>2. Binary Search ⏬ 🔗<br>3. Interpolation Search ⏬ 🔗<br>4. Exponential Search ⏬ 🔗 |
| Stacks And Queues      | 1. Implementing A Stack ⏬ 🔗<br>2. Implementing A Queue ⏬ 🔗<br>3. Priority Queue ⏬ 🔗<br>4. Circular Queue ⏬ 🔗 |
| Linked Lists           | 1. Insertion In A Linked List ⏬ 🔗<br>2. Deletion In A Linked List ⏬ 🔗<br>3. Reverse A Linked List ⏬ 🔗<br>4. Infix To Postfix Conversion ⏬ 🔗<br>5. Evaluation of Postfix Expression ⏬ 🔗<br>6. Doubly Linked List ⏬ 🔗<br>7. Circular Linked List ⏬ 🔗 |
| Trees                  | 1. Binary Tree Traversals (Inorder, Preorder, Postorder) ⏬ 🔗<br>2. Binary Search Tree (BST) Operations (Insertion, Deletion, Search) ⏬ 🔗<br>3. AVL Tree Operations ⏬ 🔗<br>4. Red-Black Tree Operations ⏬ 🔗<br>5. B-Tree Operations ⏬ 🔗 |
| Graphs                 | 1. Depth-First Search (DFS) ⏬ 🔗<br>2. Breadth-First Search (BFS) ⏬ 🔗<br>3. Dijkstra's Algorithm ⏬ 🔗<br>4. Bellman-Ford Algorithm ⏬ 🔗<br>5. Floyd-Warshall Algorithm ⏬ 🔗<br>6. Prim's Algorithm ⏬ 🔗<br>7. Kruskal's Algorithm ⏬ 🔗 |
| Recursion              | 1. Factorial Calculation ⏬ 🔗<br>2. Fibonacci Series ⏬ 🔗<br>3. Tower of Hanoi ⏬ 🔗<br>4. N-Queens Problem ⏬ 🔗 |
| Dynamic Programming    | 1. 0/1 Knapsack Problem ⏬ 🔗<br>2. Fibonacci Using Dynamic Programming ⏬ 🔗<br>3. Longest Common Subsequence ⏬ 🔗<br>4. Matrix Chain Multiplication ⏬ 🔗 |
| Hashing                | 1. Hash Table Operations (Insertion, Deletion, Search) ⏬ 🔗<br>2. Open Addressing (Linear Probing, Quadratic Probing, Double Hashing) ⏬ 🔗<br>3. Closed Addressing (Chaining) ⏬ 🔗 |
| Heap                   | 1. Heapify And Heap Sort ⏬ 🔗<br>2. Priority Queue Implementation ⏬ 🔗 |
| Bit Manipulation       | 1. Basic Bitwise Operations (AND, OR, XOR, Shifts) ⏬ 🔗<br>2. Hamming Distance ⏬ 🔗<br>3. Bitmasking Techniques ⏬ 🔗 |


## Bubble Sort Algorithm

-  **Description:**
Bubble Sort is a simple sorting algorithm that repeatedly steps through the list of elements. It compares adjacent elements and swaps them if they are in the wrong order. The pass through the list is repeated until no swaps are needed, indicating that the list is sorted.

- **Code**
Here's an example of Bubble Sort in Python:
```
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        # Traverse through the array
        for j in range(0, n-i-1):
            # Swap if the element found is greater than the next element
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]

# Example Usage:
my_list = [64, 25, 12, 22, 11]
bubble_sort(my_list)
print("Sorted array:", my_list)
```

- **Example:**
Let's say we have an unsorted list [64, 25, 12, 22, 11]. With each pass, Bubble Sort compares adjacent elements and swaps them if they're in the wrong order. It starts with [64, 25, 12, 22, 11], then [25, 12, 22, 11, 64], [12, 22, 11, 25, 64], [12, 11, 22, 25, 64], [11, 12, 22, 25, 64]. After these passes, the list is sorted.

- **Explanation:** Bubble Sort works by repeatedly moving the largest unsorted element to the end of the list. It's named "Bubble Sort" because larger elements "bubble" to the top of the list in each pass.
  
- **Note:** Bubble Sort is straightforward but may not be the most efficient sorting algorithm for large datasets. Its time complexity is O(n^2) in the average and worst-case scenarios, making it less suitable for large sets of data compared to more advanced algorithms like Merge Sort or QuickSort.

- **Limitations:**

    _Inefficiency:_ Bubble Sort has a time complexity of O(n^2), making it less efficient than other sorting algorithms for large datasets.
    _Lack of Adaptability:_ It doesn't adapt to the existing order in the list; it always compares adjacent elements.
    Not Suitable for Large Datasets: Due to its quadratic time complexity, Bubble Sort may not be practical for sorting large datasets.
