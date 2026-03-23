📘 DSA Interview Questions & Answers
1. What is a Data Structure?

Answer:
A data structure is a way to organize and store data efficiently for operations like insertion, deletion, and searching.

2. What is the difference between Array and Linked List?
Array	Linked List
Fixed size	Dynamic size
Fast access (O(1))	Slow access (O(n))
Memory contiguous	Memory scattered
3. What is Time Complexity?

Answer:
Time complexity measures how an algorithm's runtime grows with input size.

Example:

O(1) → constant
O(n) → linear
O(log n) → logarithmic
4. What is Space Complexity?

Answer:
Amount of memory used by an algorithm relative to input size.

5. What is Big-O Notation?

Answer:
It describes the worst-case performance of an algorithm.

Example:

O(n²) → nested loops
O(log n) → binary search
6. What is a Stack?

Answer:
A linear data structure that follows LIFO (Last In First Out).

Operations:

push()
pop()
peek()
7. What is a Queue?

Answer:
A linear data structure that follows FIFO (First In First Out).

Operations:

enqueue()
dequeue()
8. What is Recursion?

Answer:
A function calling itself to solve smaller subproblems.

Example:

function factorial(n){
  if(n === 0) return 1;
  return n * factorial(n-1);
}
9. What is Binary Search?

Answer:
Search algorithm for sorted arrays with O(log n).

function binarySearch(arr, target){
  let left = 0, right = arr.length - 1;

  while(left <= right){
    let mid = Math.floor((left + right) / 2);

    if(arr[mid] === target) return mid;
    else if(arr[mid] < target) left = mid + 1;
    else right = mid - 1;
  }
  return -1;
}
10. What is a Linked List?

Answer:
A collection of nodes where each node points to the next node.

11. What is a Tree?

Answer:
A hierarchical data structure with nodes and edges.

12. What is a Binary Tree?

Answer:
A tree where each node has at most 2 children.

13. What is a Binary Search Tree (BST)?

Answer:
Left child < root < right child.

14. What is DFS (Depth First Search)?

Answer:
Traverse deep before exploring neighbors.

function dfs(node){
  if(!node) return;
  console.log(node.value);
  dfs(node.left);
  dfs(node.right);
}
15. What is BFS (Breadth First Search)?

Answer:
Traverse level by level using queue.

16. What is a Hash Table?

Answer:
Stores key-value pairs for fast lookup (O(1)).

17. What is Collision in Hashing?

Answer:
When two keys map to the same index.

18. What is Dynamic Programming?

Answer:
Solving problems by storing results of subproblems.

Example:

function fib(n){
  let dp = [0,1];
  for(let i=2;i<=n;i++){
    dp[i] = dp[i-1] + dp[i-2];
  }
  return dp[n];
}
19. What is Greedy Algorithm?

Answer:
Always choose the best immediate option.

20. What is Two Pointer Technique?

Answer:
Use two indices to solve problems efficiently.

Example:

function twoSumSorted(arr, target){
  let left = 0, right = arr.length - 1;

  while(left < right){
    let sum = arr[left] + arr[right];

    if(sum === target) return [left, right];
    else if(sum < target) left++;
    else right--;
  }
}

