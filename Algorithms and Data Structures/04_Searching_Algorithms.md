# Searching Algorithms

Search methods in JavaScript:

- indexOf
- includes
- find
- findIndex

## Linear Search

- one item per time checking every single thing

## Binary Search

- rather than eliminating one element at a time you can eliminate half of the remanding elements at a time
- faster than linear
- data has to be sorted!!

## Naive String Search

Check for all character of the main string to the pattern.

## BigO for search methodes:

Linear Search:
O(1) - first element O(n)
| Method | Easiest | Normal |
| ----- | ----- | ----- |
| Linear Search | O(1) | O(n) |
| Binary Search | O(1) | O(log n) |
| Naive String Search | O(1) | O(n²) for string, O(n) for letter |
