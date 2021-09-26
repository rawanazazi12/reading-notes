# What I've Learned at the 2nd lecture of 401 code...

## Packages and Import

1. Package = directory. Java classes can be grouped together in packages. A package name is the same as the directory (folder) name which contains the .java files. 

2. Package declaration syntax
 The statement order is as follows. Comments can go anywhere.
   1. Package statment (optional).
   2. Imports (optional).
   3. Class or interface definitions.

3. Common imports
  There are 166 packages containing 3279 classes and interfaces in Java 5. However, only a few packages are used in most programming. GUI programs typically use at least the first three imports. 

   * import java.awt.*; Common GUI elements.

   * import java.awt.event.*; The most common GUI event listeners.

   * import javax.swing.*; More common GUI elements. Note "javax".

   * import java.util.*; Data structures (Collections), time, Scanner, etc classes.

   * import java.io.*; Input-output classes.
 
4. Static imports in Java 5        
   Java 5 added an import static option that allows static variables (typically constants) to be referenced without qualifying them with a class name.

## Different types of loops in Java

1. Types of loops that we can find in Java:

   * Simple for loop
   * Enhanced for-each loop
   * While loop
   * Do-While loop

2. For Loop :                                                                                                       A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.

3. While Loop:              
The while loop is Java's most fundamental loop statement. It repeats a statement or a block of statements while its controlling Boolean-expression is true.

4. Do-While Loop:      
The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.


### RESOURSES

- [Java Imports](https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html)

- [Different types of loops in Java](https://www.baeldung.com/java-loops)