## binary search
- a search algorithm that finds the position of a target element in a sorted array.
- the array is repeatedly divided 
    - half of the elements in the array is discarded during the search.
- TC: O(log n)
- Leetcode: Q35
- steps:
    - define the start and end positions of the array
    - while the start <= end
    - find the middle of the array
    - if the element at the middle index is less than the target element, increase the start index by 1
    - if the element at the middle index is greater than the target element, decrease the end index by 1;
    - if the element at the middle index equals the target element, return the middle index as the position.
    