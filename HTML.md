# Responsive Web Design
Learn HTML by Building a Cat Photo App 71 steps
https://www.freecodecamp.org/learn/2022/responsive-web-design/
Code: HTML

## Day 1 - 
<html> 
	<body>
		<main> the main is used to represent the main content of the body of the HTML document, it should be unique to the document and should not be repeated in other parts of the document.
Header : <h1> </h1> main biggest most important <h2> second most important <h3> third most important *EXAMPLE*       <h1>CatPhotoApp</h1>       <h2>Cat Photos</h2> 
Comment : <!--     --> needs to be above the <P> element *EXAMPLE*     <!-- TODO: Add link to cat photos -->
Paragraph : <p>  *EXAMPLE*       <p>Everyone loves cute cats</p> 
all elements inside the <body> are called nested elements = they should be placed two spaces further to the right of the element they are nested in (in this case the body)
image : <img> without a closing tag (void element)
HTML attributes are special words used inside the opening tag of an element to control the element's behaviour.
source : <src> attributre in an <img> element specifies the image's URL (where the image is located)
image text : <alt> text is used for screen readers if image fails to load
<img src="link goes here.jpg" alt="text"> 
Link another page with the Anchor element : (a) <p> you can add words here <a href="link" target="_blank"> text </a> you can add words here </p> *EXAMPLE* <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
To open links in a new tab, you can use the Target attribte on the anchor (a) element :   ↑target="_blank"
## Day 1 - Step > 16 done
	
<html>
  <body>
    <main>
      <h1>CatPhotoApp</h1>
      <h2>Cat Photos</h2>
      <!-- TODO: Add link to cat photos -->
      <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
      <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
      <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back.">
    </main>
  </body>
</html>
	
## Day 2 -
You can turn an image into a link by: <a href="link"> <img src="image.jpg" alt="text"> </a>
(Section) element is used to define sections in a documnent, such as chapters,headers,footers... <section> </section>
To create an (unorderdered) list of items you can use the ul element <ul> </ul> will appear as (•)
Within the <ul> element you can create <li> element to create a list in an unordered list <li> </li> *EXAMPLE*  <ul> <li> </li> </ul>
The (figure) element allows you to associate an image with a caption <figure> </figure>
A (figure caption) elemenet is used to add a caption to discribe the imagie contained within the figure element <figcaption> Text </figcaption> *EXAMPLE*  <figure> <figcaption> Text </figcaption> </figure>
To place (emphasis) on a specific word or phrase use the em element <em> </em>
To create an orderdered list <ol> </ol> and add <li> </li> will appear as (1.) (2.)
The (strong) element is used to indicate that some text is of strong importance or urgent <strong> </strong>
The (form) element is used to get information from a user like their name, email, and other details <form> </form> 
The (action) attribute indicates where form data should be sent <form action="url"></form>
The (input) element (is a void element like img) allows you several ways to collect data from a web form <input> 
There are many kinds of inputs you can create using the (type) attribute. You can easily create a password field, reset button, or a control to let users select a file from their computer. *EXAMPLE*  <input type="text"> 
In order for a form's data to be accessed by the location specified in the action attribute, you must give the text field a (name) attribute and assign it a value to represent the data being submitted. *EXAMPLE*   <input type="text" name="firstName">
(Placeholder) text is used to give people a hint about what kind of information to enter into an input.  *EXAMPLE*   <input type="text" name="firstName" placeholder="Ex. Jane Doe">
To prevent a user from submitting your form when required information is missing, you need to add the (required) attribute to an input element.  *EXAMPLE*   <input type="text" name="firstName" placeholder="Ex. Jane Doe" required>
The (button) element is used to create a clickable button. *EXAMPLE*  <button>submit</button>
To make it clear that this button does you need to add a (type)  *EXAMPLE*  <button type="submit">Submit</button> It makes your code clearer and avoids confusion with the other possible types
## Day 2 - Step > 45 done

<html>
  <body>
    <main>
      <h1>CatPhotoApp</h1>
      <section>
        <h2>Cat Photos</h2>
        <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
      <section>
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul>
          <li>catnip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
          <figcaption>Cats <em>love</em> lasagna.</figcaption>  
        </figure>
        <h3>Top 3 things cats hate:</h3>
        <ol>
          <li>flea treatment</li>
          <li>thunder</li>
          <li>other cats</li>
        </ol>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Two tabby kittens sleeping together on a couch.">
          <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
        </figure>
      </section>
      <section>
        <h2>Cat Form</h2>
        <form action="https://freecatphotoapp.com/submit-cat-photo">
 
          <input type="text" name="catphotourl" placeholder="cat photo URL" required>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
  </body>
</html>

## Day 3 -
You can use (radio) buttons for questions where you want only one answer out of multiple options. <input type="radio"> yourtextgoeshere
(label) elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers). <label><input type="radio"> yourtextgoeshere</label>
The (id) attribute is used to identify specific HTML elements. Each id attribute's value must be unique from all other id values for the entire page.     *EXAMPLE*     <label><input type="radio" id="indoor"></label>
<label><input id="indoor" type="radio" name="indoor-outdoor"> Indoor</label> we add the (name) so yyou can only selection 1 option at a time
<label><input id="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>
Add a (value) attribute to both radio button to collect valuable information
<label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
<label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
The (fieldset) element is used to group related inputs and labels together in a web form. they are block-level elements meaning that they appear on a new line. <fieldset></fieldset>
The (legend) element acts as a caption for the content in the fieldset element. It gives users context about what they should enter into that part of the form. <legend>Is your cat an indoor or outdoor cat?</legend>
The input element with a type attribute set to (checkbox) creates a checkbox. *EXAMPLE*     <input type="checkbox"> Loving  --             <input id="loving" type="checkbox"> Loving
There's another way to associate an (input) element's text with the element itself. You can nest the text within a (label) element and add a (for) attribute with the same value as the (input) element's (id) attribute.   <label for="loving">Loving</label>
In order to make a checkbox (checked) or radio button selected by default, you need to add the (checked) attribute to it. <input checked id="loving" type="checkbox" name="personality" value="loving"> <label for="loving">Loving</label>
The (footer) element is used to define a footer for a document or section. A footer typically contains information about the author of the document, copyright data, links to terms of use, contact information, and more.
After the main element, add a footer element. </main> <footer> </footer> </body>
The (head) element is used to contain metadata about the document, such as its title, links to stylesheets, and scripts. Metadata is information about the page that isn't displayed directly on the page. <html> <head> </head> <body>
The (title) element determines what browsers show in the title bar or tab for the page.    <title>CatPhotoApp</title> 
You can specify the language of your page by adding the (lang) attribute to the (html) element. <html lang="en"></lang>
All pages should begin with <!DOCTYPE html>. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.
<!DOCTYPE html> tells browsers that the document is an HTML5 document which is the latest version of HTML.
You can set browser behavior by adding (meta) elements in the (head).     <meta charset="utf-8"> It tells the browser: “Use UTF-8 encoding when reading this page.”

FULL CODE DONE:

<!DOCTYPE html>

<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>CatPhotoApp</title>
  </head>
  <body>
    <main>
      <h1>CatPhotoApp</h1>
      <section>
        <h2>Cat Photos</h2>
        <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
      <section>
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul>
          <li>catnip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
          <figcaption>Cats <em>love</em> lasagna.</figcaption>  
        </figure>
        <h3>Top 3 things cats hate:</h3>
        <ol>
          <li>flea treatment</li>
          <li>thunder</li>
          <li>other cats</li>
        </ol>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Two tabby kittens sleeping together on a couch.">
          <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
        </figure>
      </section>
      <section>
        <h2>Cat Form</h2>
        <form action="https://freecatphotoapp.com/submit-cat-photo">
          <fieldset>
            <legend>Is your cat an indoor or outdoor cat?</legend>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
          </fieldset>
          <fieldset>
            <legend>What's your cat's personality?</legend>
            <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>
            <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
            <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic">Energetic</label>
          </fieldset>
          <input type="text" name="catphotourl" placeholder="cat photo URL" required>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
    <footer>
      <p>
        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
      </p>
    </footer>
  </body>
</html>
