# Big O - Linear Time - O(n)

## Definition

Linear time is represented as O(n) and is used to describe algorithms that scale linearly with their input.

Common examples and use cases for linear time algorithms are 
* Single for loops
* Once-through *n* operations

## Example #1

``` { .cs }
public bool Contains(string[] stringArray, string targetString) {
    for (int i = 0; i < stringArray.Length; i++) {
        if (stringArray[i] == targetString) {
            return true;
        }
    }
    return false;
}
```

This algorithm has to look at each item in *stringArray* to find *targetString* and so it scales linearly with the size of the input array.

## Example #2

``` { .cs }
public ListNode GetNodeByValue(ListNode head, int targetValue) {
    ListNode currentNode = head;
    while (current != null) {
        if (current.val == targetValue) {
            return current;
        }
        current = current.next;
    }

    return null;
}
```

As with an array, this algorithm has to consider every node in the LinkedList to find the *targetValue*, so the run-time is linear with the size of the input.
