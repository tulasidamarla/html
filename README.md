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

Number input box
----------------
Number input box is used to input numbers.
    <input type="number" min="0" max="50">
    
Note: number input box only allows to enter number. It gives two caret type button to increase or decrease based on min and max. But if user manually types a value, then it is not possible to restrict. That should be handled by javascript.


Drop down list
--------------
Select tag is used for drop down selection. For ex,
    
    <select>
        <option value="Mumbai">Mumbai</option>
        <option value="Delhi">Delhi</option>
        <option value="Kolkata">Kolkata</option>
        <option value="Chennai">Chennai</option>
    </select>
    
Date 
-----
date box is used to enter date. For ex,

    <input type="date" name="journeyDate"> 
    
Note: This gives a calendar also for the user to select.    

fieldset and legend elements
----------------------------
fieldset is wraps all fields inside a box. legend is used to display a legend text on the top edge of the box. For ex,

    <fieldset>
		<legend> This is the form to be filled for trip</legend>
		<label for="firstName" > First Name:</label>
		<input id="firstName" type="text" size="20">
		<br>
		<br>
		<label for="age"> Age: </label>
		<input type="number" id="age" min="0" max="50"><br>
		<br>
    </fieldset>    

Escape characters
------------------
There are few escape characters for space(&npbsp), TM(&#8482), ampersend(&amp), copyright symbol(&copy), greater than(&gt), lesser than(&lt), quetion mark symbols(&#63), otherwise they will not be recognized by browser. 

Bold and Italic elements
------------------------
bold tag is b and italic tag is i. There is another tag <strong>text</strong> which is similar to bold but strong is used for text to speech programs, which is useful for blind people. Similarly, there is an <em>text</em> tag which is an alternate to italic tag. For ex,

	<b>bold text</b>
	<i>italic text</i>

iframe
------
iframe is nothing but another html document embedded into our web page. It is used to load data from other web pages without reloading the entire page. For ex,
	
	<iframe frameborder="1" width="200" height="200" name="firstiframe" src="sample1.html"> 
	        If you see this then your browser is not supporting iframe</iframe>
	<a href="sample2.html" target="firstiframe">Switch to document sample2</a>

sub and sup elements
---------------------
sub script and super script elements are used to raise or lower the content. For ex, in August 23rd if you want to raise the rd text above 23, we need to use sup. similarly, For H2O if we want to lower the 2, then use sup. For ex,
	
	<p>I will be on leave on August 23<sup>rd</sup> </p>
	<p> There is lot of H<sub>2</sub>O in the lake</p>
	
Title and alt attributes
------------------------
Before html 5, title attribute is restricted to few elements, but since html 5 title can be added to every tag. Basically it is used when we hover over an image, to display some text. alt attribute is used when an image is not loaded, it can display the text present in the alt attribute. For ex,
	
	<img src="mypic.JPG" title="Tulasiram" alt="Tulasiram" width="200" height="200">
	
audio element
--------------
Audio element is used to play audio on the html document. For ex,
	
	<audio controls="audiocontrols">
		<source src="gnr.mp3" type="audio/mp3">
		<!-- This will be played if mp3 is not available-->
		<source src="November Rain - Guns N Roses.wav" type="audio/wav">
	</audio>
	
Note: In HTML5, we don't need to give value to controls, we can remove the value. audio tag has other attributes like 'autoplay' , 'loop','draggable' for autoplay on load of the document, loop for continuously repeating the song and draggable(draggable="true") for dragging the audio icon.

video element
-------------
similar to audio, HTML5 has video element. The only difference is we need to mention width and height attributes in video tag. For ex,

	<video controls>
		<source src="gnr.mp4" type="video/mp4">
	</video>
