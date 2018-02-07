#### How to properly sort an array using JavaScript

###### [try it on repl.it](https://repl.it/@jasenmichael/properlySortingArrays)

```javascript
var arr = new Array(4, 11, 2, 10, 3, 1, 7, 8)  
console.log('this is arr\n', arr)
console.log('-------------')

var ASCIIsortedArr = arr.sort()
// This is ASCII character order.  
// Output: 1,10,11,2,3,4)  
console.log('sorted ASCII sortedArr\n', ASCIIsortedArr)
console.log('-------------')

// Sort the array elements with a function that compares array elements.  
arr.sort(SortAscending)
// Output: 1,2,3,4,10,11.  
console.log('sorted ascending order numerically sortedArr\n', arr)
console.log('-------------')

// Sorts array elements in ascending order numerically.  
function SortAscending(first, second)  {  

    // 1: proper long way
    // if (first == second)  
    //     return 0;  
    // if (first < second)  
    //     return -1
    // else  
    //     return 1  

    // 2: using minus
    // return first - second

    // 3: using less than(my favorite, as evaluates boolean values wrather than potentially large numbers)
    return second < first
}  


// Sort the array elements with a function that compares array elements.  
arr.sort(SortDescending)
// Output: 1,2,3,4,10,11.  
console.log('sorted descending order numerically sortedArr\n', arr)
console.log('-------------')
function SortDescending(first, second) {  
    // proper long way
    // if (first == second)  
    //     return 0;  
    // if (first < second)  
    //     return 1
    // else  
    //     return -1

    // 2: using minus
    // return second - first

    // 3: using greater than(my favorite, as evaluates boolean values wrather than potentially large numbers)
    return second > first

}
```
