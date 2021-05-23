# What I've Learned at the 2nd lecture of 201 code...

## What I've learned from the Duckett HTML book:

1. What is the purpose of using *tags* in HTML: The tags provide extra meaning 
and allow browsers to show users the appropriate structure for the page.

   - Structural Markup: the elements that you can use to describe both headings and paragraphs.

   - Semantic Markup: which provides extra information; such as where emphasis is placed in a sentence, that something 
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