# JavaScript-The-Werid-Parts


### Creation phase
Creation of an execution context
-creates global object
- creates ‘this'
- link to outer environments (if there is one)
- puts functions and variables in to memory
- vars are initially set as “undefined” and are later assigned their value (if do get assigned a value"
- The setting of variables and functions to memory is known as ‘hoisting'

####Undefined not the same as ‘not defined'
- it exists but it hasn’t been given a value yet.
- Never set variables to undefined. Leave undefined to mean you haven’t assigned the value as a programmer. If not debugging is difficult.

### Execution Phase
- Already has everything from the creations phase (global object, this etc)
- Runs your code line by line

JavaScript is single threaded and synchronous (!) in it's exception.


### Variable Environment
- where the var lives
- if the var is not defined inside its execution context, it will look for it in side its outer environment

### The Scope Chain
Reference to outer environment  depends on the the lexical environment. This is where it is defined and not invoked (‘who created me’). This reference will keep repeating until the lexical environment is the global object. This is called the scope chain.

### Scope, ES6 and Let
Let allows block scoping - meaning it’s still created and set in memory as ‘undefined’ but you cannot use until its been defined. If declared in side curly braces (block) its only available in that block.

### Asynchronous Events in Javascript
JavaScript runs synchronously, but handles async events by putting the on an events stack, it looks at these once the execution stack has finished.

###Associativity and Precedence
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence

###Coercion
coercion = converting a value from one type to another. This happens a lot in JavaScript because it is dynamically typed.
ie var a = 1 + ‘2’; is ’12’ not 2 because of coercion.
