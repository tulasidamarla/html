HTML Tutorial
-------------
Html contains tags that display text data. Everytag has a closing tag. For ex, 
    
    <body>some text</body>.

Note: The tags together with data inside it is called markup element. <br>
Note: There are few tags you don't need an end tag. they are called empty tag. For ex, 
  
    <br> 
is a line break. It doesn't need end element because we are not writing anything in between. one br tag gives one line spacing in the document. If you want one character spacing, use nbsp. i.e.

    &nbsp
    
Lists
-----
There are two types of lists. Ordered lists(ol tag) and Unordered lists(ul tag). ol tags are less frequently used. Both ul and ol tags have a child tag li. li means list item. The difference between ol and ul is ol list items are given numbering where as ul list items are displayed with bullets.

Creating Weblinks
-----------------
To create weblink to anchor tag is used. For ex to create a link for an external website:
    
    <a href="www.youtube.com">Go to Youtube </a>
    
If you want to create a link to different sections with in the same page:
    
    <a href="#Section1">Go to Section1</a>

The section1 should be defined like this:
    
    <a name="Section1">This is Section1 </a>

Image tag
---------
To render an image on the document use img tag. For ex,
    
    <img src="abc.jpg">

Note: img is also an empty tag, because you don't need any text to be displayed. you can resize the image by specifying height and width attributes.

Input tag
---------
Input tags are for user to enter, select something for server side rendering of data. These elements come under form tag. For ex,

    <form action="/login" method="GET">
        <input type="text" name="userName" size = "20">
    </form>
 
Note: Input is another empty tag. There are different input elements like text, radio button, select, submit etc.

Label tag
---------
Label tags are used to label different html elements. More often input elements. For ex,
    
    <label for="firstName" > First Name:</label>
    <input id="firstName" type="text">

Note: for attribute of label tag should match id attribute of input tag. so when we click on label, it will take the cursor to the input element.

textarea
---------
textarea tag is used for entering multiline text. unlike input it is not an empty element. Ex:
    
    <textarea rows="20" cols="40"></textarea>

Radio Button and check boxes
----------------------------
Both radio button and check boxes are used for taking serveys, preferences etc from the user. Radio button is mutually excluse, where as check boxes are multi select. For ex,
    
    yes:
    <input type="radio" name="prefergames" value="yes">
    no:
    <input type="radio" name="prefergames" value="no">
    <input type="checkbox" name="" checked="checked" >Foot ball <br>
    <input type="checkbox" name="" >Basket ball <br>
    <input type="checkbox" name="" >Cricket <br>

Note: name attribute should be same, otherwise both radio buttons are treated seperately. In checkbox, if checked attribute set to "checked", that is checked by default on page load.


