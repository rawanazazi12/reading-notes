# What I've Learned at the 8th lecture of 201 code

## CSS Layout

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


**RESOURSES:**

- [Book1](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2FHTML%20CSS%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRVRES1VTSXQ5QnhLbWw5Mm5lUXFzTG9CN1dUTEZPNzB2Y3NtUThJLUhsUlRFUT9ydGltZT1BQ1lpYnhvZTJVZw)
