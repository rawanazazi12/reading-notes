# What I've Learned at the 1st lecture of 301 code...


## Components

**Component Based Architecture**

1. The primary objective of component-based architecture is to ensure component reusability.

2. Component-oriented software design has many advantages over the traditional object-oriented approaches such as:

     * Reduced time in market and the development cost by reusing existing components.
     * Increased reliability with the reuse of the existing components.

3. **What is a Component?**                
A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.

4. A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities.

5. **What are the charactistics of a component?**

    * *Reusability*: Components are usually designed to be reused in different situations in different applications

    * *Replaceable*: Components may be freely substituted with other similar components.

    * *Not context specific*: Components are designed to operate in different environments and contexts.

    * *Extensible*: A component can be extended from existing components to provide new behavior.

    * *Encapsulated*: A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

    * *Independent*: Components are designed to have minimal dependencies on other components.

6. **What are the advantages of using component based architecture?**

    * Ease of deployment.

    * Reduced cost.

    * Ease of development.

    * Reusable.

    * Reliability.

    * Independent.


## What is Props and How to Use it in React

1. **What is props short for?**       

**Props**is a special keyword in React, which stands for properties and is being used for passing data from one component to another.


2. Props data is read-only, which means that data coming from the parent should not be changed by child components.
3. **How are props used in React?**

   1. Firstly, define an attribute and its value(data).
   2. Then pass it to child component(s) by using Props
   3. Finally, render the Props Data.

4. Props are being passed to components like function arguments.

5. **What is the flow of props?** 

Props can only be passed to components in one-way (parent to child).

6. Props data is immutable (read-only).


## Things I want to know more about:

I want to know more about props and how it exactly works.

## RESOURSES

- [Component Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

- [What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)

- [Components and Props](https://reactjs.org/docs/components-and-props.html)

