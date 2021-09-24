# What I've Learned at the 1st lecture of 401 code...

## Java Basics

### Variables

* The Java programming language defines the following kinds of variables:

   1. *Instance Variables* (Non-Static Fields) Technically speaking, objects store their individual states in "non-static fields", that is, fields declared without the static keyword.

   2. *Class Variables* (Static Fields) A class variable is any field declared with the static modifier; this tells the compiler that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated.

   3. *Local Variables* Similar to how an object stores its state in fields, a method will often store its temporary state in local variables. The syntax for declaring a local variable is similar to declaring a field (for example, int count = 0;).

   4. *Parameters* You've already seen examples of parameters, both in the Bicycle class and in the main method of the "Hello World!" application.

### Operators

   1. relational : < > <= >= instanceof
   2. equality : == !=
   3. bitwise AND : &
   4. bitwise exclusive OR : ^
   5. bitwise inclusive OR : |
   6. logical AND : &&
   7. logical OR : ||
   8. ternary : ? :
   9. assignment : = += -= *= /= %= &= ^= |= <<= >>= >>>=

### Control Flow Statements

 The statements inside your source files are generally executed from top to bottom, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. This section describes the decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.