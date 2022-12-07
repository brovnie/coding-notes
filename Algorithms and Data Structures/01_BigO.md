#BigO

**Big O Notation** is a way of describing the relationship between the input to a function or as it grows and how that changes the runtime of that function, the relatinship between the input size and the time relative to that input.

We say that an algorithm is O(f(n))) if the number of simple operations the computer has to do is eventually less than a constant times f(n), as n increases

f(n) could be:

- linear (f(n) = n)
- quadratic (f(n) = n(power2))
- constant (f(n) = 1 )
- something entirely different
  <sub>f(n) - operation
  n - time</sub>

  Examples:

**O(1)**

```javascript
function sumOfIntegers(n) {
  return (n * (n + 1)) / 2;
}
```

3 operations[* + /] => O(1)

**O(n)**

```javascript
function sumOfIntegers(n) {
  let total = 0;
  for (let i = 1; i <= n; i++) {
    total += i;
  }
  return total;
}
```

Number of operations is (eventually) bounded by multiple a of n
[i++, total+=, loop] => O(n)

**O(n²)**

```javascript
function printPairsOfNumbers(n) {
  for (var i = 0; i < n; i++) {
    for (var j = 0; j < n; j++) {
      console.log(i, j);
    }
  }
}
```

O(n) operation inside O(n) operation [nested loops]

** Space Complexity in JS **

- Most primitives (booleans, numbers, undefined, null) are constant space
- Strings require O(n) space (where n is the string length)
- Reference types are generally O(n), where n is the key length (for arrays) of the number of keys (for objects)

** Performance of arrays and objects **

- Object \* - unorderd data structures where everything is stored in key value pairs
  Big O of Objects

  - Insertion - O(1)
  - Removal - O(1)
  - Searching - O(N)
  - Access - O(1)

  Big O of Object Methods

  - Object.keys - O(N)
  - Object.values - O(N)
  - Object.entries - O(N)
  - hasOwnProperty - O(1)

- Arrays \* - ordered list

Big of Arrays

- Insertion - It depends
- Removal - It depends
- Searching - O(N)
- Access = O(1)
  <sub>Adding/removing from the beginning of the array is heavier because all items from array has to by moved by 1 or -1 and the key has to be adjusted </sub>

Big O of Arrays Methods

- push - O(1)
- pop - O(1)
- shift - O(N)
- unshift - O(N)
- concat - O(N)
- slice - O(N)
- splice - O(N)
- sort - O(N \* log N)
- forEach/map/filter/reduce/etc. - O(N)
