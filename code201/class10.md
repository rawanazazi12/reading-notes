# What I've Learned at the 10th lecture of 201 code

## Duckett JS book

### Chapter10:  Debugging

1. **ORDER OF EXECUTION** : To find the source of an error, it helps to know how scripts are processed.
 The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

2. **EXECUTION CONTEXTS**
 The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.

3. **EXECUTION CONTEXT & HOISTING**
 Each time a script enters a new execution context, there are two phases of activity:

   1. *PREPARE*  

         - The new scope is created.
         - Variables, functions, and arguments are created.
         - The value of the this keyword is determined.

   2. *EXECUTE*
        - Now it can assign values to variables.
        - Reference functions and run their code.
        - Execute statements.

4. **UNDERSTANDING SCOPE**
 In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it.Each execution context can also access its parent's v a ri ables object.

5. **UNDERSTANDING ERRORS**
 If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

6. **ERROR OBJECTS**
 Error objects can help you find where your mistakes are and browsers have tools to help you read them.

7. **HOW TO DEAL WITH ERRORS**

    1. DEBUG THE SCRIPT TO FIX ERRORS.

    2. HANDLE ERRORS GRACEFULLY.

8. *TYPING IN THE CONSOLE IN CHROME*
  You can just type code into the console and it will show you a result.

9. **BREAKPOINTS**

    You can pause the execution of a script on any line using breakpoints. Then you can check the 
    values stored in variables at that point in time. 

10. **HANDLING EXCEPTIONS**

    If you know your code might fail, use try, catch, and finally. Each one is given its own code block.

11. **THROWING ERRORS**

    If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.

12. **COMMON ERRORS**

     - GO BACK TO BASICS.

     - MISSED/ EXTRA CHARACTERS.

     - DATA TYPE ISSUES.

13. If you understand execution contexts (which have two stages) and stacks, you are more likely to find the error in    your code.

14. Debugging is the process of finding errors. It involves a process of deduction.

15. The console helps narrow down the area in which the error is located, so you can try to find the exact error.

16. JavaScript has 7 different types of errors. Each creates its own error object, which can tell you its line number and gives a description of the error.

17. If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.
Use them to give your users helpful feedback.


### RESOURSES

 - [JS Book](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2Fjavascript%5Fand%5Fjquery%5Finteractive%5Fjon%5Fdu%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRWNpeDhSX2FtUVZQaFJwblB5SmFTbW9CbGVObG9CeGd0amduYlhTN1Q5TWdvQT9ydGltZT1hNEVuYnhvZTJVZw)




