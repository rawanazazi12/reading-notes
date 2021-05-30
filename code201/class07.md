# What I've Learned at the 7th lecture of 201 code

1. **Tables:**
*What’s a Table?*
A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.
2. TABLES
The `< table >` element is used to add tables to a web page.
   - A table is drawn out row by row. Each row is created with the `< tr >` element.
3. Inside each row there are a number of cells represented by the `< td>` element `(or < th>` if it is a header).
4. You can make cells of a table span more than one row or column using the rowspan and colspan attributes.
5. For long tables you can split the table into a `< thead>`,`< tbody >`, and `< tfoot>`.
6. DATA TYPES REVISITED In JavaScript there are six data types: Five of them are described as simple (or primitive) data types. The sixth is the object (and is referred to as a complex data type).
7. SIMPLE OR PRIMITIVE DATA TYPES JavaScript has five simple (or primitive) data types:
   - String
   - Number
   - Boolean
   - Undefined (a variable that has been declared, but no value has been assigned to it yet).
   - Null (a variable with no value - it may have had one at some point, but no longer has a value) both the web browser and the current document can be modeled using objects (and objects can have methods and properties). But it can be confusing to discover that a simple value (like a string, a number, or a Boolean) can have methods and properties.
   
8. **JavaScript** treats every variable as an object in its own right. String: If a variable, or the property of an object, contains a string, you can use the properties and methods of the String object on it. Number: If a variable, or property of an object, stores a number.
9. you can use the properties and methods of the Number object on itBoolean: There is a Boo 1 ean object. It is rarely used. (Undefined and null values do not have objects.)
10. COMPLEX DATA TYPE JavaScript also defines a complex data type: 6.0bject Under the hood, arrays and functions are considered types of objects.
11. *ARRAYS ARE OBJECTS* As you saw on p118, an array is a set of key/value pairs (just like any other object). But you do not specify the name in the key/value pair of an array - it is an index number. like other objects, arrays have properties and methods.
12. There is also a set of methods you can use with any array to add items to it, remove items from it, or reorder its contents.
13. FUNCTIONS ARE OBJECTS Technically, functions are also objects. But they have an additional feature: they are callable, which means you can tell the interpreter when you want to execute the statements that it contains.


**RESOURSES:**

- [Resource1](https://github.com/codefellows/domain_modeling#domain-modeling)
- [Resourse2](https://alqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2Fjavascript%5Fand%5Fjquery%5Finteractive%5Fjon%5Fdu%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRWNpeDhSX2FtUVZQaFJwblB5SmFTbW9CbGVObG9CeGd0amduYlhTN1Q5TWdvQT9ydGltZT1hNEVuYnhvZTJVZw)