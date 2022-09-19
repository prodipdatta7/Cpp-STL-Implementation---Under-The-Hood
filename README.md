# Cpp STL Implementation | Under The Hood
 
|STL|Internal Implementation|Time Complexity of methods|
|---|---|---|
|[unordered_set](https://en.cppreference.com/w/cpp/container/unordered_set)|Hash Table where keys are hashed into indices of a hash table so that the insertion is always randomized| Best: O(1), Worst: O(n) depends on internally used hash function|
|[set](https://en.cppreference.com/w/cpp/container/set)|Red Black Tree| Insertion, deletion, search: O(n)|
|[unordered_map](https://en.cppreference.com/w/cpp/container/unordered_map)|Hash Table|O(1)|
|[map](https://en.cppreference.com/w/cpp/container/map)|Red Black self balancing binary search tree| Insertion, deletion, search: O(n)|
|[stack](https://en.cppreference.com/w/cpp/container/stack)|Can be implemented using array, list, dequeue| push, pop, top: O(1)|
|[sort](https://en.cppreference.com/w/cpp/algorithm/sort)|intro sort: insertion sort + quick sort + heap sort; 1. Input size is larger then quick sort if it takes more time then switched to heap sort, 2. input size is smaller then insertion sort|O(nlogn)|
|[queue](https://en.cppreference.com/w/cpp/container/queue), [dequeue](https://en.cppreference.com/w/cpp/container/deque), [circulur queue](https://www.geeksforgeeks.org/circular-queue-set-1-introduction-array-implementation/)|Using array or list|Insert, Remove, Size: O(1)|
|[priority_queue](https://en.cppreference.com/w/cpp/container/priority_queue)|heap|Insertion: O(logn), top: O(1)|