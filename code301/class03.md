# What I've Learned at the 3rd lecture of 301 code...

## React Docs - lists and keys

1. **What does .map() return?**                           
map() returns a new array with length equal to the original array.

2. **If I want to loop through an array and display each value in JSX, how do I do that in React?**                     
Using .map() which iterates through an array and calls a specified function for each of the items.

3. **Each list item needs a unique** _Key___.

4. **What is the purpose of a key?**         
 Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity.


 ## The Spread Operator

 1. **What is the spread operator?**                  
 The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a functionβs arguments.

2. **List 4 things that the spread operator can do.**

   1. *Copying an array*
   2. *Concatenating or combining arrays*
   3. *Using an array as arguments*
   4. *Combining objects*

3. **Give an example of using the spread operator to combine two arrays.**      
  >const myArray = [`π€ͺ`,`π»`,`π`]
   const yourArray = [`π`,`π€`,`π€©`]
   const ourArray = [...myArray,...yourArray]
   console.log(...ourArray) // π€ͺ π» π π π€ π€©  

 >
4. **Give an example of using the spread operator to add a new item to an array.**

 >const fewFruit = ['π','π','π']            
  const fewMoreFruit = ['π', 'π', ...fewFruit]             
  console.log(fewMoreFruit) //  Array(5) [ "π", "π", "π", "π", "π" ]         
>

5. **Give an example of using the spread operator to combine two objects into one.**

 The spread syntax is useful for combining the properties and methods on objects into a new object:      
  >onst objectOne = {hello: "π€ͺ"}            
  const objectTwo = {world: "π»"}                     
  const objectThree = {...objectOne, ...objectTwo, laugh: "π"}                
  console.log(objectThree) // Object { hello: "π€ͺ", world: "π»", laugh: "π" }                    
  const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("π".repeat(5))}}                     
  objectFour.laugh() // πππππ     

 >

## How to Pass Functions Between Components

1. **In your own words, what does the increment function do?**             
It's updating the state by incrementing the count if the name matches the one that passed to the function.

2. **How can you pass a method from a parent component into a child component?**           
Using props 

3. **How does the child component invoke a method that was passed to it from a parent component?**

   Passing data from child to parent by employing callbacks.

## Things I want to know more about                 
I want to practice more with passing methods from parent into a child and the opposite.


## RESOURSES             
- [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

- [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

- [How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

