# What I've Learned at the 2nd lecture of 301 code...

## React lifecycle

1. **What are component lifecycle events?**            
React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. 

2. **Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**     
*componentDidMount* will only be called once after the first *render*.

![diagram](https://miro.medium.com/max/2000/0*0saPKFiTUk6W3FYp)

3. **What is the very first thing to happen in the lifecycle of React?**         
The `static getDerivedStateFromProps`, is the first React lifecycle method to be invoked during the updating phase.

4. Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`

    2. `React Updates`
    1. `constructor`
    3. `render`
    4. `componentDidMount`
    5. `componentWillUnmount`

5. **What does componentDidMount do?**         
The componentDidMount() method allows us to execute the React code when the component is already placed in the DOM (Document Object Model). This method is called during the Mounting phase of the React Life-cycle i.e after the component is rendered.

## React State Vs Props

1. **What types of things can you pass in the props?**                    
 Props in React allows us to pass values from a parent component down to a child component. The values can be any data type, from strings to functions, objects, etc.

2. **What is the big difference between props and state?**          
*State* is handled in the component and you can update it inside the component.                       
*Prps* are handled outside the component and must be updated outside of the component
![propsVsstate](https://i.stack.imgur.com/wqvF2.png)

3. **When do we re-render our application?**

   React components automatically re-render whenever there is a change in their state or props.


4. **What are some examples of things that we could store in state?**                
Variables that we want to changing or updating them.


## Things I want to know more about

I want to learn more about using react bootstrap and how to style my whole page using it .

## RESOURSES

- [React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

- [React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

