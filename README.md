# IPL Project

## Best Practices: Imports

When you import a module, always name the module the same as the file name or it's installed module name. That way it becomes easier to debug when the code becomes more complex.

If you are using [destructuring](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment), this is does not work out.

Bad Usage:
```javascript

 const functions = require("./ipl");
 functions.mostManOfTheMatch();

 ````

 Good Usage:
 ```javascript

 const ipl = require("./ipl");
 ipl.mostManOfTheMatch();

 ```