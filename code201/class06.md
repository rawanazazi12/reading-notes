# What I've Learned at the 6th lecture of 201 code

## Understanding The Problem Domain Is The Hardest Part Of Programming Article

1. What is the hardest thing about writing code

   - Learning a new technology
   - Naming things
   - Testing your code
   - Debugging
   - Fixing bugs
   - Making software maintainable

2. Programming is easy if you understand the problem domain.

3. > If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

    - Make the problem domain easier.

    - Get better at understanding the problem domain.

## What I've learned from the Duckett JS book:

1. WHAT IS AN OBJECT:

   Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

2. IN AN OBJECT: Variables become known as properties.

3. IN AN OBJECT: Functions become known as methods.

4. Creating an object:
   Literal Notation: The easiest and most popular way to create objects.

5. DOM: The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

6. MAKING A MODEL OF THE HTML PAGE: When the browser loads a web page, it creates a model of the page in memory.

7. ACCESSING AND CHANGING THE HTML PAGE: The DOM also defines methods and properties to access and update each object in  this model, which in turn updates what the user sees in the browser.

8. THE DOM TREE IS A MODEL OF A WEB PAGE: As a browser loads a web page, it creates a model of that page. 
The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes.

9. WORKING WITH THE DOM TREE:
   Accessing and updating the DOM tree involves two steps:
   1. Locate the node that represents the element you want to work with.
   2. Use its text content, child elements, and attributes.

10. ACCESSING ELEMENTS:

    **DOM** queries may return one element, or they may return a Nodelist, which is a collection of nodes.

11. *SELECTING AN ELEMENT FROM A NODELIST:*

  There are two ways to select an element from a Nodelist: *The item() method* and *array syntax*. Both require the index number of the element you want.

12. The browser represents the page using a DOM tree.

13. DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.

14. You can select element nodes by their id or cl ass attributes, by tag name, or using CSS selector syntax.

15. Whenever a DOM query can return more than one node, it will always return a Nade list.

16. From an element node, you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques.

17. An element node can contain multiple text nodes and child elements that are siblings of each other.

18. In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).

19. Browsers offer tools for viewing the DOM tree .


**RESOURSES:**

- [Resource1](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)
- [Resourse2](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2Fjavascript%5Fand%5Fjquery%5Finteractive%5Fjon%5Fdu%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRWNpeDhSX2FtUVZQaFJwblB5SmFTbW9CbGVObG9CeGd0amduYlhTN1Q5TWdvQT9ydGltZT1hNEVuYnhvZTJVZw)


