# Recursion #

* Recursion * process that calls itself.
Redurs functions call themsels.

```javascript
function recursion(endpoint) {
    if(endpoint > 1) {
        return recursion()
    }
    endpoint++;
}
```
## How do funcions work? ##

In almost all programming languages there is a build in data structure that manages what happends when functions are invoked - *call stack*
<sub> *Call stak* is stack data structure. </sub>
Any time a function is invoked it is placed on the top of the call stack
When JS sees the return keyword or when the function ends the compiler will remove function from the call stack(pop)
In recursief function the function is beeing pushed into call stact and is removed when it meet the breakpoint and returns the value

## Helping method recursion ##
```javascript
function output(input) {
    let outerScopeValue= [];
    
    function helper(helperInput) {
        helper(helperInput--);
    }
    helper(input);

    return outerScopeVariable;
}
```