# Images in HTML

*A picture can say a thousand words, and great images help make the difference between an average-looking site and a really engaging one*

Adding Images ***< img >*** must carry two attributes: 
* ***src*** in order to tell the browser where it can find the image file
* ***alt*** provides a text description of the image


### Rules for creating images
* Saving images in the right **format** jpeg, gif, or png
* Saving images at the right **size** in order not to be distorted and stretched.
* Using the correct **resolution** images created for the web should be saved at a resolution of 72 ppi


# Colors in CSS

There are many ways to specify colors in CSS:

* ### **Color names** (common names) "***color: Cyan***"
* ### **HEX codes** (six-digit codes) "***color: #ffffff***"
* ### **RGB values** (red, green and blue) "***color: rgb(10,30,50)***"
* ### **HSL values** (hue, saturation and lightness) "***color: hsl(0,100%,100%)***"



# Text in CSS

### Fonts Typefaces
* **Serif** letters have extra details
* **Sans-Serif** letters have straight ends and clean design
* **Monospace** letters have the same width.
* **Cursive** letters like handwriting styles
* **Fantasy** letters are decorative and used for titles


|       **Function**       |            **Property**            |                               **Details**                                     |
|--------------------------|------------------------------------|-------------------------------------------------------------------------------|
| **Specifying Typefaces** | ***font-family***                  | the value is the name of a typeface                                           |
| **Size**                 | ***font-size***                    | using pixels, percentages, or ems. (16px = 100% = 1em)                        |
| **Importance**           | ***font-weight***                  | to create bold text                                                           |
| **Style**                | ***font-style***                   | to create italic text                                                         |
| **Capitalize**           | ***text-transform***               | to change the case of text with value: uppercase, or lowercase, or capitalize |
| **Decoration**           | ***text-decoration***              | with value: none, or line-through, or blink                                   |
| **Spacing**              | ***letter-spacing, word-spacing*** | to change the space between letters and words                                 |
| **Alignment**            | ***text-align***                   | to control the alignment of text                                              |


### pseudo-elements

|       **Function**       |                                 **Details**                                              |     **Property**    |                                 Details                                      |
|--------------------------|------------------------------------------------------------------------------------------|---------------------|------------------------------------------------------------------------------|
| **First Letter or Line** | to specify different values for the first letter or first line of text inside an element | ***:first-letter*** |                                                                              |
|                          |                                                                                          | ***:first-line***   |                                                                              |
|                          |                                                                                          |               |                                                                              |
| **Styling links**        | to set different styles for links that have and have not yet been visited                | ***:link***         | to set styles for links that have not yet been visited                       |
|                          |                                                                                          | ***:visited***      | to set styles for links that have been clicked on                            |
|                          |                                                                                          |               |                                                                              |
| **Responding to users**  | to change the appearance of elements when a user is interacting with them                | ***:hover***        | applied when hovering over an element with a pointing device such as a mouse |
|                          |                                                                                          | ***:active***       | applied when an element is being activated                                   |
|                          |                                                                                          | ***:focus***        | applied when an element has a focus                                          |


### Attribute Selectors



|        **Selector**        |                                 **Meaning**                                        |            **Form**               |
|----------------------------|------------------------------------------------------------------------------------|-----------------------------------|
| ***[]***     **Existence** | Matches a specific attribute (whatever its value)                                  | ***element [ attr ]***            |
| ***[ = ]***  **Equality**  | Matches a specific attribute with a specific value                                 | ***element [ attr =  "value" ]*** |
| ***[ ~= ]*** **Space**     | Matches a specific attribute whose value appears in a spaceseparated list of words | ***element [ attr ~= "value" ]*** |
| ***[ ^= ]*** **Prefix**    | Matches a specific attribute whose value begins with a specific string             | ***element [ attr ^ "letter" ]*** |
| ***[ *= ]*** **Substring** | Matches a specific attribute whose value contains a specific substring             | ***element [ attr * "letter" ]*** |
| ***[ $= ]*** **Suffix**    | Matches a specific attribute whose value ends with a specific string               | ***element [ attr $ "letter" ]*** |

 

   
  
 
  


 

  

  

  

  

  

  



