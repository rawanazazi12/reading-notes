# What I've Learned at the 10th lecture of 301 code...


##  JavaScript Call Stack 

1. What is a ‘call’?                 
   A call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

2. What does LIFO mean?

   (LIFO) principle to temporarily store and manage function invocation (call).

3. How many ‘calls’ can happen at once?           
   The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution).

4. What causes a Stack Overflow?                       
   A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error. 

## JavaScript error messages

1. What is a ‘refrence error’?                 
   In JavaScript, a reference error is thrown when a code attempts to reference a non-existing variable.

2. What is a ‘syntax error’?                 
   An exception caused by the incorrect use of a pre-defined syntax. Syntax errors are detected while compiling or parsing source code.
  
3. What is a ‘range error’?          
   A RangeError is thrown when trying to pass a value as an argument to a function that does not allow a range that includes the value.    

4. What is a ‘type error’?             
   TypeError object represents an error when an operation could not be performed, typically (but not exclusively) when a value is not of the expected type.
           
5. What is a breakpoint?                 
   At each breakpoint, JavaScript will stop executing, and let you examine JavaScript values.     

6. What does the word ‘debugger’ do in your code?
   Debuggers are used to identify coding errors at various development stages.



### Things I want to know more about

  I want to learn more about tracking errors, to be able to deal with errors and fix them without taking too much time.

### RESOURSES

 - [Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/) 

  - [JavaScript error messages](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)




