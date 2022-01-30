# Scope

## Global Scope
    - available everywhere in the code.

## Local Scope
    - only available within the function in which it is defined.

eg.

```javascript
let myGlobalVar = "global";

const printMyVars = function() {
  let myLocalVar = "local";
  console.log("-- Inside printMyVars --");
  console.log("myLocalVar is:", myLocalVar);
  console.log("myGlobalVar is:", myGlobalVar);
}

printMyVars();

console.log('-- Outside of printMyVars now --');
console.log(myLocalVar);
```

Scoping can override variables

1 - The local variable (myVar) takes precedence inside myFunction. 
2 - It would evaluate to "local"
3 - However outside the function the variable myVar behaves as a global variable. It would evaluate to "global"

### Rule 5 for defining functions

It is ideal if functions try to avoid reading outer scope variables. 
If a function needs some information / data, then that **data should instead be passed in as a parameter,** making it available within the **function's inner scope.**