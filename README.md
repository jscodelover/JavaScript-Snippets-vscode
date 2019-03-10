# JavaScript snippets

---

This extension contains code snippets for JavaScript syntax for [Vs Code](https://code.visualstudio.com/) editor.

## Snippets

Below is a list of all available snippets.

### Function

`nfn`→ create a funtion with function keyword `function functionName () {}`
`fn`→ create a anonymous function `function () {}`
`afn`→ create a arrow function `const functionName= () => {}`
`apply`→ create an apply funtion `functionName.apply(this,arguments)`
`call`→ create a call function `functionName.call(this,arguments)`
`iife`→ create iife function `(function() {} ();)`
`iifer`→ create iife function with return value `const result=(function(){ return ; } ();)`

### Array Methods

`arrmth`→ create array method for - forEach, map, filter, find, every, some.
`reduce`→ create array method`iterable.(forEach,map,filter,find,every,some)(item => {})`

### Conditional Operator

`i`→ Basic if statment `if(conditon) {}`
`ife`→ If-else statment `if(conditon) {} else {}`
`ei`→ Else if statment `else if(condition) {}`
`swt`→ Switch Statment

```
   switch(expression){
    case condition: //...
                    break;
    case condition: //...
                    break;
    default: //....
   }
```

### Loops

`fin`→ For in loop `for(const key in source) {}`
`fof`→ For of loop `for(cont key of source) {}`
`wl`→ while loop `while(condition) {}`

### Fetch Request

`fetch`→ Fetch Request

```
fetch('url')
    .then(res => res.json())
    .then(data => console.log(data));
```

`fetchc`→ Fetch with catch

```
fetch('url')
    .then(response => {
        if (response.status === 200) {
            return response.json();
        } else {
            throw new Error('Something went wrong on api server!');
        }
    })
    .then(data => {
        console.debug(data);
    }).catch(error => {
        console.error(error);
    });
```

`asyncfetch`→ Async/Await Fetch Request

```
const request = async () => {
    const response = await fetch('url');
    const data = await response.json();
    console.log(data);
}
```

### Exception Handling

`tc` Try and Catch `try {} catch(err) {}`
`tcf` Try, Catch and Finally `try {} catch(err) {} finally {}`
