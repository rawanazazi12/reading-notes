# What I've Learned at the 4th lecture of 301 code...


## React Docs - Forms

1. **Forms**                  
 HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state. 

2. **What is a ‘Controlled Component’?**               
 An input form element whose value is controlled by React.

3. **Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**             
  We should update the state with their responses as soon as they enter them, cause we need these values to be used at the moment the user submitted the form.

4. **How do we target what the user is entering if we have an event handler on an input field?**        
 Using event.target.value


1. **Why would we use a ternary operator?**             
 Using ternary operartor allows us to refactor our code and excute the same thing, but writing shorter code, a one line code instead of multiple lines.


2. **Rewrite the following statement using a ternary statement:**
     >  if(x===y){                           
     console.log(true);                    
     } else {                          
     console.log(false);                       
     }
    >

    `if(x===y)? console.log(true): console.log(false);`


## Things I want to know more about             
  I want to know more about sort() method and when I need to use it.



### RESOURSES

- [React Docs - Forms](https://reactjs.org/docs/forms.html)

- [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)


