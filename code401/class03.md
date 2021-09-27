# What I've Learned at the 3rd lecture of 401 code...

## Primitives vs. Objects

1. Java Type System                           
  Java has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean. Every primitive type corresponds to a reference type.

2. The process of converting a primitive type to a reference one is called autoboxing, the opposite process is called unboxing.

3. The reference types are objects, they live on the heap and are relatively slow to access. They have a certain overhead concerning their primitive counterparts.

4. Performance                     
  The performance of a Java code is quite a subtle issue, it depends very much on the hardware on which the code runs, on the compiler that might perform certain optimizations, on the state of the virtual machine, on the activity of other processes in the operating system.

5. Default Values
  Default values of the primitive types are 0 (in the corresponding representation, i.e. 0, 0.0d etc) for numeric types, false for the boolean type, \u0000 for the char type. For the wrapper classes, the default value is null.

## Scanning

1. Objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

2. Breaking Input into Tokens
  By default, a scanner uses white space to separate tokens. (White space characters include blanks, tabs, and line terminators. 

3. Translating Individual Tokens
  The ScanXan example treats all input tokens as simple String values. Scanner also supports tokens for all of the Java language's primitive types (except for char), as well as BigInteger and BigDecimal. Also, numeric values can use thousands separators.


## Exceptions

1. What Is an Exception?                  
  An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

2. How to Throw Exceptions                  
  Using the throw statement and the Throwable class and its subclasses.
 
3. Advantages of Exceptions                        
  The use of exceptions to manage errors has some advantages over traditional error-management techniques. You'll learn more in this section.


### RESOURSES

- [Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)

- [Exceptions](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)

- [Scanning](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)

