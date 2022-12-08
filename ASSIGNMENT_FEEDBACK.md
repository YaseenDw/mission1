Hi Yaseen!

As you can see below there are a few things to work on.

The main issues are the contact form and the responisveness. Follow the link below for ideas on how to fix the contact form, and add the meta tag for the viewport to set a responsive context, then look at how the page is reendered.

The mobile menu needs to be fixed, I've described one way it can be done below but it can be a bit tricky. We did something similar in one of the early lectures - week3, in a file called images.html with a matching css.file. We made a hiden div that would slide in when another div is hovered.

Please fix these things up, psuh your changes to gthub and let me know when I should have another look.

*************************************

CRITERIA FOR GRADING

*************************************

GODKÄNT:
-------------------------------------

3 separate pages: ✅

A header with a page title on every page: ✅❌
  The contact page doesnöt have a title. Google looks for a unique h1 tag on every page

A navigational menu every page with links to the other pages: ❌ ✅
  Mobile menu doesn't work. You need to add a hover pseudo class to .navbar-toggle 
  and use css sibling selectors to target the menu. 

Contact form:
    Email: ✅
    Message: ❌
    Required: ❌
    Mail to: ❌
    Add a message field.
    Add the "required" attribute to each input
    Add an action to the form. Have a look at this for a guide: https://www.w3schools.com/html/tryit.asp?filename=tryhtml_form_mail

RWD:
    Desktop: ✅
    Mobile: ❌
      Add <meta name="viewport" content="width=device-width, initial-scale=1.0">
      to the head section of each page to set a responsive context 

External CSS: ✅

-------------------------------------

VÄLGODKÄNT:
-------------------------------------

Current page indication in the menu: ❌
  Add an "active" class to each menu item on the relevant page to style it

Responsive Image: ❌
  Set a width: 100%; on the image on the home page. 

RWD:
  Media Query: ✅
  Flex/Grid: ✅

Separate CSS: ✅ ❌
  Although you have separate files, there is a lot of duplicated content in those files. The first 90 lines in each CSS file are the same. A better approach is to put all the common styling into one file - "general.css" or some thing like that, then just have the page specific styles in each file. In the head section of the html pages you can import mpore than one css file

  Semantic: ✅❌
  All the header andd nav stuff is semantic, but .hihi, .yas etc doesn't tell the reader what those divs are for.

Semantic Element naming: ✅❌
   See above

Code Style:
  HTML: ❌ ✅
  Header and navigation is ok, some odd indentation and empty lines but not too bad.
  After that it gets messy, with no indenttatin and mismatched opening and closing tags example from shoes.html line 35:

<section id="h">
<div class="hehe">
<h1 class="haha">de bästa i gamet</h1>
<p class="hihi">de mesta populära</p>
<img src="images/hihi.webp" class="huhu">
</section>
</div>
<button class="btn">see more</button>
</body>
</html>


  CSS: ✅ ❌
  Pretty good, but a css selector should always have a space before the opening {  and an empty line after the closing }. Example from themenu.css:

  .yaydiv{
    display:flex;
    align-items: center;
    justify-content: center;
    border-style: dotted;
    color:#0b080c;
    background-color: #fff;
}
.yas{
width: 50%;
height: 100%;
display: flex;
flex-wrap: wrap;
align-items: center;
justify-content: left;
}

should be:

.yaydiv {
    display:flex;
    align-items: center;
    justify-content: center;
    border-style: dotted;
    color:#0b080c;
    background-color: #fff;
}

.yas {
    width: 50%;
    height: 100%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: left;
}

