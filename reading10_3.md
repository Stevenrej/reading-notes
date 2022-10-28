# Understanding the JavaScript Call Stack

1. What is a ‘call’? - function invocation
2. How many ‘calls’ can happen at once? - a single, function(s) execution
3. What does LIFO mean? - Last In, First Out
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
5. What causes a Stack Overflow? - A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## JavaScript error messages

1. What is a ‘reference error’? - This is as simple as when you try to use a variable that is not yet declared you get this type os errors.
2. What is a ‘syntax error’? - I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
3. What is a ‘range error’? - Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.
4. What is a ‘type error’? - Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.
5. What is a breakpoint? - When you want stop your code fro running at a certain point
6. What does the word ‘debugger’ do in your code? - displays all information related to running and debugging and has a top bar with debugging commands and configuration settings

[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)