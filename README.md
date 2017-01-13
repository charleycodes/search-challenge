# Search an array of sorted numbers.


items    : An array of sorted ints, with no duplicates
n_items  : Number of elements in the items array
ascending: non-zero if the array is sorted in ascending order
key      : the key to search for
type     : the type of match to find

This function finds the element in the array that best fits the search criteria. It returns the match type and the index of the matching item.

**LessThan**:  Finds the largest item which is less than the key.  It returns FoundLess if a match is found, NotFound if no match is found.

**LessThanEquals**:  Finds the item which is equal to the key, or the largest item which is less than the key. Returns FoundExact if an item that exactly matches the key is found, FoundLess if a non-exact match is found and NotFound if no match is found.

**Equals**:  Finds an item which is equal to the key. Returns FoundExact if an item if found, NotFound otherwise.

**GreaterThanEquals**:  Finds the item which is equal to the key, or the smallest item which is greater than the key. Returns FoundExact if an item that exactly matches the key is found, FoundGreater if a non-exact match is found and NotFound if no match is found.

**GreaterThan**:  Finds the smallest item which is greater than the key. Returns FoundGreater if a match if found, NotFound if no match is found.


**Examples**:

Given the input array `[0, 2, 4, 6, 8]` (ascending order)

+-----+-------------------+--------------+-------+
| Key | Type              | Returns      | Index |
+-----+-------------------+--------------+-------+
| -1  | LessThanEquals    | NotFound     | X     |
+-----+-------------------+--------------+-------+
|  0  | LessThan          | NotFound     | X     |
+-----+-------------------+--------------+-------+
|  0  | Equals            | FoundExact   | 0     |
+-----+-------------------+--------------+-------+
|  1  | Equals            | NotFound     | X     |
+-----+-------------------+--------------+-------+
|  2  | GreaterThanEquals | FoundExact   | 1     |
+-----+-------------------+--------------+-------+
|  2  | GreaterThan       | FoundGreater | 2     |
+-----+-------------------+--------------+-------+


Given the input array `[8, 6, 4, 2, 0]` (descending order)

+-----+-------------------+--------------+-------+
| Key | Type              | Returns      | Index |
+-----+-------------------+--------------+-------+
| -1  | LessThan          | NotFound     | X     |
+-----+-------------------+--------------+-------+
|  0  | LessThan          | NotFound     | X     |
+-----+-------------------+--------------+-------+
|  4  | LessThanEquals    | FoundExact   | 2     |
+-----+-------------------+--------------+-------+
|  8  | Equals            | FoundExact   | 0     |
+-----+-------------------+--------------+-------+
|  5  | GreaterThanEquals | FoundGreater | 1     |
+-----+-------------------+--------------+-------+
|  2  | GreaterThanEquals | FoundExact   | 3     |
+-----+-------------------+--------------+-------+
|  8  | GreaterThan       | NotFound     | X     |
+-----+-------------------+--------------+-------+
|  9  | GreaterThan       | NotFound     | X     |
+-----+-------------------+--------------+-------+


**Assumptions**:  
- The items are sorted
- Items will be non-NULL
- There are no duplicate items
- n_items will be > 0

## <a name="technologies"></a>Technologies
Tech Stack: Python<br/>

## <a name="features"></a>Features

Search an array of sorted items.


## <a name="install"></a>Installation

To run the search:

Clone or fork this repo:

```
https://github.com/CharleyMcLean/search-challenge.git
```

Run the app:

```
python -i challenge.py
```
