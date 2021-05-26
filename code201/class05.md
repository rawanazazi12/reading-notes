# What I've Learned at the 5th lecture of 201 code

## What I've learned from the Duckett HTML book

### Chapter 5: “Images” (pp.94-125)

1. Choosing Images for a site: A picture can say a thousand words, and great images help make the difference between an
average-looking site and a really engaging one.

2. Images should...
   - Be relevant
   - Convey information
   - Convey the right mood
   - Be instantly recognisable
   - Fit the color palette

3. Adding Images to a site:

   - *< img >* To add an image into the page you need to use an < img > element.

   - *src* : This tells the browser where it can find the image file. This will usually be a relative URL pointing to an  image on your own site.

   - *alt* : This provides a text description of the image which describes the image if you cannot see it.

   - *title* : You can also use the title attribute with the < img > element to provide additional information about the  image

4. Height & Width of Images:

   - *Height* :This specifies the height of the image in pixels.

   - *Width* : This specifies the width of the image in pixels.

5. Where to Place Images in Your Code :

   1. before a paragraph.

   2. inside the start of a paragraph.

   3. in the middle of a paragraph.

6. Three Rules for Creating Images:

   1. Save images in the right format.

   2. Save images at the right size.

   3. Save images at the right size.

7. Tools to Edit & Save Images: There are several tools you can use to edit and save images to ensure that they are the right size, format, and resolution.

   - The most popular tool amongst web professionals is **Adobe Photoshop**.

8. Image Formats:

   - **JPEG** Whenever you have many different colors in a picture you should use a JPEG.

   - **GIF**

   - Use **GIF** or **PNG** format when saving images with few colors or large areas of the same color.

9. Image Dimensions : The images you use on your website should be saved at the same width and height that you want them to appear on the page.

10. Cropping Images : When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.

11. Image Resolution : Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.

12. Vector Images : Vector images differ from bitmap images and are resolution-independent. Vector images are commonly created in programs such as Adobe Illustrator.

13. Animated GIFs : Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.

14. Transparency : Creating an image that is partially transparent (or "see-through") for the web involves
selecting one of two formats:

    - Transparent GIF

    - PNG

15. Examining Images on the Web:

    1. Checking the Size of Images

    2. Downloading Images

16. HTML5: Figure and Figure Caption:

    - `<figure>` images often come with captions. HTML5 has introduced a new `<figure>` element to contain images and their caption so that the two are associated.

    - `<figcaption>` The `<figcaption>` element has been added to HTML5 in order to allow web page authors to add a caption to an image.

17. You must always specify a src attribute to indicate the source of an image and an alt attribute to describe the
content of an image.

18. You should save images at the size you will be using them on the web page and in the appropriate format.

19. You should save images at the size you will be using them on the web page and in the appropriate format.

### Chapter 11: “Color” (pp.246-263)

1. *Foreground Color*
   The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

    1. rgb values
    2. hex codes
    3. color names

2. *Background Color*
   background-color : CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.

3. *Understanding Color* : Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

4. *Contrast* : When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

   - Low Contrast
   - High Contrast
   - Medium Contrast

5. *CSS3: HSL Colors* : CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and  lightness values.

6. *CSS3: HSL & HSLA*

7. It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).

8. CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.

9. CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.

### Chapter 12: “Text” (pp.264-299)

1. *Typeface Terminology* :
   - Serif
   - Sans-Serif
   - Monospace

2. There are properties to control the choice of font, size, weight, style, and spacing.

3. There is a limited choice of fonts that you can assume most people will have installed.

4. If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.

5. You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.

6. You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

7. *Attribute Selectors*

     |  Selector      |   Meaning  |
     | ----------- | ------------|
     |Existence|`[]` Matches a specific attribute (whatever its value)|
     |Equality |`[=]` Matches a specific attribute with a specific value|
     |Space |`[~=]` Matches a specific attribute whose value appears in a spaceseparated list of words|
     |Prefix |`[^=]` Matches a specific attribute whose value begins with a specific string|
     |SubString |`[*=]` Matches a specific attribute whose value contains a specific substring|

### JPEG vs PNG vs GIF

**JPEG vs PNG vs GIF — which image format to use and when?**

   - There are hundreds of image formats available each with a specific use case. I bet most of us wouldn’t have come across 90% of the image formats listed on Wikipedia.

   - *Transparency*
      >In a simple form, transparency indicates something that is completely invisible. Logos and icons often need to be placed on backgrounds with variable colours. Hence it is desirable, that the background of these logos and icons is made transparent so that a single image can be used over multiple background variations.

   - *JPEG* images don’t support transparency and are hence not usable for such cases.

   - *GIF* images support transparency by declaring a single colour in the colour palette as transparent (inde        transparency).
