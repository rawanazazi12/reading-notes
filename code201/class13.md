# What I've Learned at the 13th lecture of 201 code

1. **LOCAL STORAGE**    
  Local storage is one of the areas where native client applications have held an advantage over web applications.

2. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.

3. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).

4. Cookies are limited to about 4 KB of data — enough to slow down your application , but not enough to be terribly useful.

5. **HTML5 Storage**     
 It’s a way for web pages to store named key/value pairs locally, within the client web browser.

6. From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object. Before you can use it, you should detect whether the browser supports it.

7. Check for HTML5 Storage: 
 
     >function supports_html5_storage() {        
     try {         
     return 'localStorage' in window && window['localStorage'] !== null;       
     } catch (e) {          
     return false;        
     }            
     }       

8. Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage.     
   `Modernizr.localstorage`

9. **USING HTML5 STORAGE**     
  HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats.

10.  >interface Storage {     
      getter any getItem(in DOMString key);      
     setter creator void setItem(in DOMString key, in any data);    
     };  

11. TRACKING CHANGES TO THE HTML5 STORAGE AREA : If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.

12. **STORAGEEVENT OBJECT**

     |  PROPERTY      |   TYPE	  | DESCRIPTION	  |
     | ----------- | ------------|------------|
     |key|string|	the named key that was added, removed, or modified|
     |oldValue |any	|the previous value (now overwritten), or null if a new item was added|
     |newValue |any	|the new value, or null if an item was removed|
     |url* |string	|the page which called a method that triggered this change|


## RESOURSES

  - [Local Storage for Web Applications](http://diveinto.html5doctor.com/storage.html#history)