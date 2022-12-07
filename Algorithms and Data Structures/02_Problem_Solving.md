** Algorithm ** is a process of set of steps to accomplish a certain task.

## Problem Solving strategies:

1. Understand the Problem
2. Explore Concrete Examples
3. Break It Down
4. Solve Or Simplify
5. Look Back and Refactor
   <sub>_How to Solve It_ George Polya</sub>

### Understand the Problem

Steps:

1. Restate the problem in your own words
2. Find inputs that go into the problem
3. Defind the expected output (ex. what value, type should be returned)
4. Determinate if given inputs can defind the expected output. What information is missing?
5. Label the importand pieces of data

### Explore Concrete Examples

Examples provide sanity checks that your eventual solution works how it should.
User Stories and Unit Tests can be used to check the solution.
Tips:

- Start with simple examples
- Progress tp more complex examples
- Explore examples with empty inputs
- Explore examples with invalid inputs

### Break It Down

Explicity write out the steps you need to take.

## Solve Or Simplify

Simplify steps:

- Find the core difficulty in what you are trying to do
- Temporalry ignore that
- Write a simplified solution
- Incorporate that difficulty back in

## Look Back and Refactor

Questions:

- Can you check the result?
- Can you derive the solution differently?
- Can you understand it at a glance?
- Can you use the result of method for some other problem?
- Can you improve the performance of your solution
- Can you think of other ways to refactor?
- How have other people solved this problem?

### Problem Solving Patterns

Patterns:

- Frequency Counter
- Multiple Pointers
- Sliding Window
- Divide and Conquer
- Dynamic Programming
- Greedy Algorithms
- Backtracking
- ...

** Frequency Counter ** uses objects or sets to collect values/frequencief of values.
This can often avoid the need for nexted loops or O(N²) operations with arrays/strings

** Multiple Pointers ** is about creating pointers or values that correspond to and index or position and move towards the beginning, end and middle based on a certain condition. It's very efficient for solving problems with minimul space coplexity as well.

** Sliding Window ** this pattern involves creating a window which can either ba an array or number for one position to another. Depending on a certain condition the window either increases or closes (and a new window is created). It's very useful for keeping track of a subset of data in an array/string etc.

** Devide and Conquer ** this pattern involves dividing a data set into smaller chunks and then repeating a process with a subset of data. This pattern can tremendously decrease time complexity.
