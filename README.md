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

`tc`→ Try and Catch `try {} catch(err) {}`
`tcf`→ Try, Catch and Finally `try {} catch(err) {} finally {}`

### Axios

`ax`→ Axios Request for all get, post, put, delete

```
axios.(get,post,put,delete)('url')
    .then(res => console.log(res.data))
    .catch(err => console.log(err));
```

`asyncax`→ Axios Request for all get, post, put, delete

```
async function functionName() {
    try {
      const response = await axios.(get,post,put,delete)('url');
      const data = await response.json();
      return data;
    } catch (error) {
      console.log(error);
    }
}
```

### Timer

`st`→ Set Timeout `setTimeout(() => {}, delay)`
`si`→ Set Interval `setInterval(() => {}, intervalInms)`
`sim`→ Set Immediate `setImmediate(() => {})`
`stv`→ Set TimeOut with variable `const timer = setTimeout(() => {}, delay)`
`ct`→ Clear Timeout `clearTimeout(variableName)`  
`siv`→ Set Interval with variable `cont timer = setInterval(() => {}, intervalInms)`
`ci`→ Clear Interval `clearInterval(variableName)`

### Destructure

`ad`→ Array Destructure `const [element1, element2] = array`
`od`→ Object Destructure `const {property1, property2} = object`

### ES6 Modules

`e`→ export `export member`
`ed`→ export default `export default member`
`edf`→ export default named function `export default function functionName() {}`
`ec`→ export const `export const member = value`
`im`→ import `import * from 'module'`  
`ima`→ import as `import * as name from 'module'`
`imd`→ import with destructure `import { } from 'module'`  
`rq`→ require `const module = require(module)`
`me`→ module exports `module.exports = {}`

### Class

`cls`→ class

```
class name {
    constructor() {
    }
}
```

`clsx`→ class with extends

```
class name extends base {
    constructor() {
      super();
    }
}
```

### Console

`clog`→ console.log `console.log(obj);`
`cl`→ console log with key value pair `console.log('obj:',obj);`
`cclr`→ console clear `console.clear();`
`cw`→ console warn `console.warn(obj);`
`ctb`→ console table `console.table(obj);`
`cass`→ console assert `console.assert(expression, obj);`
`cc`→ console count `console.count(label);`
`ccr`→ console countrest `console.countReset(label);`
`cdir`→ console dir `console.dir(obj, {colors: true, depth: null});`
`cerr`→ console error `console.error(obj);`
`cgrp`→ console group `console.group(label);`
`cend`→ console groupend `console.groupEnd();`
`cin`→ console info `console.info(obj)`
`ctym`→ console time `console.time(label);`
`cte`→ console timeend `console.timeEnd(label);`
`ctg`→ console timelog `console.timeLog(label);`
`ctr`→ console trace `console.trace(label);`
