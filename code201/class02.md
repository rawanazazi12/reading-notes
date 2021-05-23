# What I've Learned at the 2nd lecture of 201 code...

### What I've learned from the Duckett HTML book:

1. What is the purpose of using *tags* in HTML: The tags provide extra meaning 
   and allow browsers to show users the appropriate structure for the page.

   - *Structural Markup:* the elements that you can use to describe both headings and paragraphs.

   - *Semantic Markup:* which provides extra information; such as where emphasis is placed in a sentence, that something 
    you have written is a quotation.
 
2. **Headings**: HTML has six "levels" of 
   headings: < h1 > to,< h6 > , for example:  

   - < h1 > is used for main headings.
   - < h2 > is used for subheadings.     

    If there are further sections under the subheadings then the < h3 > element is used, and so on.

3. **Paragraphs**: A paragraph consists of one or more sentences that form a self-contained unit of discourse.   
    The start of a paragraph is indicated by a new line.
   - < p > paragraph tag < /p > .

4. **Bold** & *Italic* :
   - By enclosing words in the tags < b > and < /b > we can make characters appear bold.
   - By enclosing words in the tags < i > and < /i > we can make characters appear italic.

5. **Superscript & Subscript** :
   - The < sup > element is used to contain characters that should be superscript such 
    as the suffixes of dates or mathematical concepts like raising a number to a power such as 22.
   - The < sub > element is used to contain characters that should be subscript. It is commonly 
    used with foot notes or chemical formulas such as H2O.

6. **White Space** :      
  In order to make code easier to read, web page authors often add extra spaces or start some 
  elements on new lines.When the browser comes across two or more spaces next to each other, it only displays one space.

7. **Line Breaks & Horizontal Rules** :
   - < br /> : the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag < br /> .

   - < hr /> : To create a break between themes — such as a change of topic in a book or a new scene  
   in a play — you can add a horizontal rule between sections using the < hr /> tag.

8. **Strong & Emphasis** :
   - < strong > : The use of the < strong >element indicates that its content has strong importance. 
   For example, the words contained in this element might be said with strong emphasis.

   - < em > : The < em > element indicates emphasis that subtly changes the meaning of a sentence.

9. **Quotations** :
   - < blockquote > : The < blockquote > element is used for longer quotes that take up an entire paragraph. 
   - < q > : The < q > element is used for shorter quotes that sit within a paragraph. 

10. **Citations & Definitions** :     

    - < cite > : When you are referencing a piece of work such as a book, film or research paper, the  
    < cite > element can be used to indicate where the citation is from.

    - < dfn > : The < dfn > element is used to indicate the defining instance of a new term.

11. **Author Details** :
    - < address > : The < address > element has quite a specific use to contain contact details for the author of 
    the page.
    - It can contain a physical address, but it does not have to. For example, it may also contain a 
    phone number or email address.

12. **Changes to Content** :
    - < ins > < del > : The < ins > element can be used to show content that has been inserted into a document, while 
    the < del > element can show text that has been deleted from it.
    - < s > : The < s > element indicates something that is no longer accurate or relevant (but that 
    should not be deleted).

13. **HTML elements** :
    - used to describe the structure of the page (e.g. headings, subheadings, paragraphs).
    - They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).

14. **CSS** : 
     - CSS allows you to create rules that specify how the content of an element should appear.
     - CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.

15. *Three ways for adding CSS :*
     - Using External CSS : using < link > tag ,The < link > element can be used in an HTML document to tell the browser where to find the CSS file used to style the page. 
     - Using Internal CSS : using < style > tag,You can also include CSS rules within an HTML page by placing them inside 
     a < style > element, which usually sits inside the < head > element of the page. 
     - Inline CSS : using style attribute in the same line of the tag, for example : < p style="color:red;">< /p >

16. **CSS Selectors** :

     |  Selector      |   Meaning  |
     | ----------- | ------------| 
     |Universal Selector|Applies to all elements in the document|
     |Type Selector |Matches element names|
     |Class Selector |Matches an element whose class attribute has a value that matches the one specified after theperiod (or full stop) symbol|
     |ID Selector |Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol|
     |Child Selector |Matches an element that is a direct child of another|
          



17. **CSS** treats each HTML element as if it appears inside its own box and uses rules to indicate how that 
    element should look.

18. Different types of selectors allow you to target your rules at different elements.

19. **CSS** rules usually appear in a separate document, although they may appear within an HTML page.


### What I've learned from the Duckett JS book:

1. A *script* is made up of a series of statements. Each statement is like a step in a recipe.

2. Scripts contain very precise instructions. For example, you might specify that a value must be remembered 
before creating a calculation using that value.

3. Variables are used to temporarily store pieces of information used in the script.

4. Arrays are special types of variables that store more than one piece of related information.

5. JavaScript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false).

6. Expressions evaluate into a single value.

7. Expressions rely on operators to calculate a value.

8. **Comparison operators:** Comparison operators are used in logical statements to determine equality or difference    between variables or values.

     |  Operator	      |   Description  |
     | ----------- | ------------| 
     | ==	|equal to|
     |=== |equal value and equal type|
     |!= |not equal|
     |!== |not equal value or not equal type|
     |> |greater than	|
     |< |less than		|
     |>= |greater than or equal to|
     |<= |less than or equal to	|


 *For extra information you can go through these links* :

  - [Book1](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2FHTML%20CSS%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRVRES1VTSXQ5QnhLbWw5Mm5lUXFzTG9CN1dUTEZPNzB2Y3NtUThJLUhsUlRFUT9ydGltZT1BQ1lpYnhvZTJVZw)


  - [Book2](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2Fjavascript%5Fand%5Fjquery%5Finteractive%5Fjon%5Fdu%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRWNpeDhSX2FtUVZQaFJwblB5SmFTbW9CbGVObG9CeGd0amduYlhTN1Q5TWdvQT9ydGltZT1hNEVuYnhvZTJVZw)