#### How to properly sort an array using JavaScript

###### [try it on repl.it](https://repl.it/@jasenmichael/properlySortingArrays)

```javascript
var arr = new Array(4, 11, 2, 10, 3, 1)  
console.log('this is arr\n', arr)
console.log('-------------')

var ASCIIsortedArr = arr.sort()
// This is ASCII character order.  
// Output: 1,10,11,2,3,4)  
console.log('sorted ASCII sortedArr\n', ASCIIsortedArr)
console.log('-------------')


// Sort the array elements with a function that compares array elements.  
b = arr.sort(CompareForSort) 
// Output: 1,2,3,4,10,11.  
console.log('sorted ascending order numerically sortedArr\n', arr)
console.log('-------------')

// Sorts array elements in ascending order numerically.  
function CompareForSort(first, second)  
{  
    if (first == second)  
        return 0;  
    if (first < second)  
        return -1
    else  
        return 1  
}
```
