# JavaScript-The-Werid-Parts


###1) Creation phase
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

###2) Execution Phase
- Already has everything from the creations phase (global object, this etc)
- Runs your code line by line

JavaScript is single threaded and synchronous (!) in it's exception.
