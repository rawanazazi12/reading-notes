# What I've Learned at the 4th lecture of 201 code...

## What I've learned from the Duckett HTML book:

1. *Writing Links* :Links are created using the < a > element. Users can click on anything between the opening < a > tag and the closing < /a > tag. You specify which page you want to link to using the href attribute.  
 < a  href="URL">IMDB< /a >

2. *Relative URLs* : Relative URLs can be used when linking to pages within our own website. They provide a shorthand way of telling the browser where to find our files.

3. *Directory Structure* :On larger websites it's a good idea to organize our code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.

   - Structure
   - Homepages
   - Relationships

4. When a website is live (that is, uploaded to a web server) we may see a couple of other techniques used that do not 
work when the files are on our local computer.

5. A forward slash will return the homepage for the entire site, and a forward slash followed by a file name will return that file providing it is in the root directory.

6. *Email Links*
To create a link that starts up the user's email program and addresses an email to a specified email address, you use the < a >element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to.

7. Opening Links in a New Window : 
**Target**  If you want a link to open in a new window, you can use the target attribute on the opening < a > tag. The value of this attribute should be **_blank** .

8. If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.

9. You can create links to open email programs with an email address in the "to" field.

10. You can use the id attribute to target elements within a page that can be linked to.

11. **Building Blocks** :CSS treats each HTML element as if it is in its own box. This box will either be a block-level
box or an inline box.

     - *Block-level elements* : start on a new line. Ex: < h1 >, < p >, < ul >, < li >


     - *Inline elements* : flow in between surrounding text. Ex: < img >, < b >, < i >


12. Controlling the Position of Elements: CSS has the following positioning schemes that allow you to control the layout of a page: **normal flow**, **relative positioning**, and **absolute positioning**. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.

13. To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.

14. *Normal Flow* : In normal flow, each block-level element sits on top of the next one.

15. *Relative Positioning* : Relative positioning moves an element in relation to where it would have been in normal flow.


16. *Absolute Positioning* : When the position property is given a value of absolute, the box is taken out of normal 
flow and no longer affects the position of other elements on the page.

17. *Fixed Positioning* : Fixed positioning is a type of absolute positioning that requires the position property 
to have a value of fixed.


## What I've learned from the Duckett JS book:

1. **WHAT IS A FUNCTION**: Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

2. **JavaScript Function Syntax** :A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().
Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).
The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...).

3. **Function parameters** are listed inside the parentheses () in the function definition.

4. **Function arguments** are the values received by the function when it is invoked.

5. Inside the function, the arguments (the parameters) behave as local variables.

6. **Calling Function** The code inside the function will execute when "something" invokes (calls) the function:

     - When an event occurs (when a user clicks a button)
     - When it is invoked (called) from JavaScript code
     - Automatically (self invoked)

7. **Function Return** When JavaScript reaches a return statement, the function will stop executing.

8. If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking    statement.

9. Functions often compute a return value. The return value is "returned" back to the "caller"

10. *Why Functions?* 
    - You can reuse code: Define the code once, and use it many times.

    - You can use the same code many times with different arguments, to produce different results.

11. How does pair programming work?
 
    While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer.

12. Why pair program?
    While learning to code, developers likely study several programming languages. Similar to a foreign language class, there are four fundamental skills that help anyone learn a new language: Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea Reading: understanding what written language intends to convey Writing: producing from scratch a meaningful.

13. **6 Reasons for Pair Programmin** :
    
    1. Greater efficiency.
    2. Engaged collaboration.
    3. Learning from fellow students.
    4. Social skills.
    5. Job interview readiness.
    6. Work environment readiness.




    ***RESOURSES***

      - [Book1](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2FHTML%20CSS%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRVRES1VTSXQ5QnhLbWw5Mm5lUXFzTG9CN1dUTEZPNzB2Y3NtUThJLUhsUlRFUT9ydGltZT1BQ1lpYnhvZTJVZw)


      - [Book2](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2Fjavascript%5Fand%5Fjquery%5Finteractive%5Fjon%5Fdu%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRWNpeDhSX2FtUVZQaFJwblB5SmFTbW9CbGVObG9CeGd0amduYlhTN1Q5TWdvQT9ydGltZT1hNEVuYnhvZTJVZw)

      - [pair programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)







    


