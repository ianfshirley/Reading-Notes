## In Memory Storage

### Understanding the JavaScript Call Stack

1. What is a ‘call’?
- function invocation
2. How many ‘calls’ can happen at once?
- one at a time
3. What does LIFO mean?
- Last in, first out. last function pushed into the stack is the first one to pop out when the function returns
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
- 
5. What causes a Stack Overflow?
- a recursive function (a function that calls itself) without an exit point. 

### JavaScript error messages

1. What is a ‘reference error’?
- when you try to use a variable that's not yet declared
2. What is a ‘syntax error’?
- when you have something that cannot be parsed. code is using the wrong syntax (has something unnecessary or missing something that is necessary)
3. What is a ‘range error’?
- when you try to manipulate an object with length and give it an invalid length (like a negative length for an array)
4. What is a ‘type error’?
- types of data are incompatible (string, number etc.)
5. What is a breakpoint?
- A point where JS stops executing
6. What does the word ‘debugger’ do in your code?
- lets you see the history before reaching that breakpoint. it lets you know what was being executed before getting to that point.

### Sources

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)<br>
[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)<br>
[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)<br>