# What I've Learned at the 3rd lecture of 201 code...

## What I've learned from the Duckett HTML book:

1. **HTML** provides us with three different types of lists:

   - *Ordered lists* (< ol >< /ol >) : are lists where each item in the list is numbered. For example, the list might be a set of steps   for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a sectionnumber.
   - *Unordered lists* (< ul >< /ul >) : are lists that begin with a bullet point (rather than characters that indicate order).
   - *Definition lists* (< dl >< /dl >): are made up of a set of terms along with the definitions for each of those terms.

2. *Nested lists* : You can put a second list inside an < li > element to create a sublist or nested list.

3. Lists can be nested inside one another.

4. Box dimensions: width,height By default a box is sized just big enough to hold its contents. To set your own       dimensions for a box you can use the height and width properties.

5. The most popular ways to specify the size of a box are to use:
   *pixels*, *percentages*, or *ems*. Traditionally, **pixels have been the most popular method because they allow designers to accurately control their size**.

6. **Overflow** :The overflow property tells the browser what to do if the content contained within a box is larger than  the box itself.

7. **Border**, **Margin** & **Padding** :Every box has three available properties that can be adjusted to control its appearance:
   1. *Border* : Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border 
   separates the edge of one box from another.
   2. *Margin* : Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.
   3. *Padding* : Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.

8. **Border Width** : The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values:
   1. thin
   2. medium
   3. thick

9. **Border Style** :You can control the style of a border using the border-style property.
   This property can take the following values:
   - solid
   - dotted
   - dashed
   - double
   - groove
   - ridge

10. **Border Color** : You can specify the color of a border using either RGB values, hex codes or CSS color names.

11. **Change Inline/Block** :The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. The values this property can take are :

    - inline
    - block
    - inline-block
    - none
12. CSS treats each HTML element as if it has its own box. 
13. You can use CSS to control the dimensions of a box.
14. You can also control the borders, margin and padding for each box with CSS.
15. It is possible to hide elements using the display and visibility properties.
16. Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
17. Legibility can be improved by controlling the width of boxes containing text and the leading.

## What I've learned from the Duckett JS book:

1. **Data Types**: JavaScript distinguishes between numbers, strings, and true or false values known as Booleans.

2. Scripts contain very precise instructions. For example, you might specify that a value must be remembered 
before creating a calculation using that value. 

3. *Variables* are used to temporarily store pieces of information used in the script.

4. *Arrays* are special types of variables that store more than one piece of related information.

5. **JavaScript** distinguishes between numbers (0-9), strings (text), and Boolean values (true or false).

6. *Expressions* evaluate into a single value.

7. *Expressions* rely on operators to calculate a value.

8. **The if Statement** : Used to specify a block of JavaScript code to be executed if a condition is true.  
  Syntax : if (condition) {
           //  block of code to be executed if the condition is true
                }
9. **The if else Statement** :Used to specify a new condition if the first condition is false.   
   Syntax : if (condition1) {
            //  block of code to be executed if condition1 is true
            } else if (condition2) {//  block of code to be executed if the condition1 is false and condition2 is true
            } else { //  block of code to be executed if the condition1 is false and condition2 is false}

10. **Switch statement** : A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 

    Syntax : switch (level) { case 'One ': title= 'Level 1 ' ;     
                              break;    
                              case 'Two':   
                              tit 1 e = ' Level 2';   
                              break;    
                              case ' Three' :   
                              title = 'Level 3'    ; 
                              break ;   
                              default :  
                              title= 'Test';   
                              break; 

11. **Loops** are handy, if you want to run the same code over and over again, each time with a different value.
      JavaScript supports different kinds of loops:

      - for - loops through a block of code a number of times. 
      - for/in - loops through the properties of an object.
      - for/of - loops through the values of an iterable object.
      - while - loops through a block of code while a specified condition is true.
      - do/while - also loops through a block of code while a specified condition is true.

12. Conditional statements allow your code to make decisions about what to do next.

13. if ... else statements allow you to run one set of code if a condition is true, and another if it is false.

14. switch statements allow you to compare a value against possible outcomes (and also provides a defaultoption if none   match).

15. Data types can be coerced from one type to another. 

16. All values evaluate to either truthy or falsy.

17. There are three types of loop: for, while, and do ... while. Each repeats a set of statements.


*For extra information you can go through these links* :

  - [Book1](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2FHTML%20CSS%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRVRES1VTSXQ5QnhLbWw5Mm5lUXFzTG9CN1dUTEZPNzB2Y3NtUThJLUhsUlRFUT9ydGltZT1BQ1lpYnhvZTJVZw)


  - [Book2](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2Fjavascript%5Fand%5Fjquery%5Finteractive%5Fjon%5Fdu%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRWNpeDhSX2FtUVZQaFJwblB5SmFTbW9CbGVObG9CeGd0amduYlhTN1Q5TWdvQT9ydGltZT1hNEVuYnhvZTJVZw)