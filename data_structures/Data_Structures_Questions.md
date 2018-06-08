Add your answers to the questions below.

1. What is the runtime complexity of your `depthFirstForEach` method?

O(n). Cb is called once for each item in tree

2. What is the space complexity of your `depthFirstForEach` function?

O(1). No additional space is necessary, purely recursive definition

3. What is the runtime complexity of your `breadthFirstForEach` method?

O(n). Every node is visited

4. What is the space complexity of your `breadthFirstForEach` method? 

O(2h), where h is the depth of the tree. Each node must store its 2 children in a queue before continuing. The queue will eventually hold 2h items when the bottom level is being processed.

5. What is the runtime complexity of your `heapsort` function?

O(2n * logn) or O(n * logn). The heap is filled in n operations of logn complexity (insert is logn) and then drained in n operations of logn complexity (delete is also logn, worst case). 

6. What is the space complexity of the `heapsort` function? Recall that your implementation should return a new array with the sorted data. What would be the space complexity if your function instead altered the input array?

O(2n). Building the heap takes n spots in memory, and the resulting output array also takes n spots.
