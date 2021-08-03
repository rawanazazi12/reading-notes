# What I've Learned at the 9th lecture of 301 code...

## Functional Programming Concepts

1. What is functional programming?
 
    Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.


2. What is a pure function and how do we know if something is a pure function?
    
   - It returns the same result if given the same arguments (it is also referred as deterministic).

   - It does not cause any observable side effects.

3. What are the benefits of a pure function?                  
   The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts.

4. What is immutability?              
   Unchanging over time or unable to be changed.

5. What is Referential transparency?            
   A function consistently yields the same result for the same input.

## Node JS- Modules and require()

1. What is a module?
   - A module is just a file. One script is one module. As simple as that.

   - Modules can load each other and use special directives export and import to interchange functionality, call functions of one module from another one.
 
2. What does the word ‘require’ do?            
   `require` function is the easiest way to include modules that exist in separate files.
   
3. How do we bring another module into the file the we are working in?                   
   Using require.

4. What do we have to do to make a module available?              
   Using the module.exports 

 
## Things I want to know more about              
   I wanna learn more about modules and how to use them in backend.

### RESOURSES
  
  - [Functional Programming](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa) 

  - [Node.js- Modules](https://www.youtube.com/watch?v=xHLd36QoS4k)

