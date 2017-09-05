# MDN: Learn web development

## Getting started with the Web

### Getting started with the Web overview

### Installing basic software

*Grunt* or *Gulp* to automatically perform repetitive tasks, such as minifying code and running tests.

### What will your website look like?

### Dealing with files

Name folders and files completely in lowercase with no spaces.

* Many computers, particularly web servers, are case-sensitive.
* Browsers, web servers, and programming languages do not handle spaces consistently.

It's better to separate words with dashes, rather than underscores.

What structure should your website have?

* index.html
* images/
* styles/
* scripts/

### HTML basics

HTML contains six heading levels, \<h1\>–\<h6\> although you'll commonly only use 3–4 at most.

    <h1>My main title</h1>
    <h2>My top level heading</h2>
    <h3>My subheading</h3>
    <h4>My sub-subheading</h4>

The most common list types are ordered and unordered lists:

* Unordered lists are wrapped in a \<ul\> element.
* Ordered lists are wrapped in an \<ol\> element.

Each item inside the lists is put inside an \<li\> (list item) element.

    <ul> 
        <li>technologists</li>
        <li>thinkers</li>
        <li>builders</li>
    </ul>

To add a link, we need to use a simple element — \<a\> — the "a" being short for "anchor". *href* stands for *hypertext reference*.

    <a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>

### CSS basics

CSS (Cascading Style Sheets) is the code you use to style your webpage.

The whole structure of a basic unit in CSS is called a rule set (but often "rule" for short).

You can also select multiple types of elements and apply a single rule set to all of them. Include multiple selectors separated by commas.

    p,li,h1 {
        color: red;
    }

Different types of selector

* p: Selects \<p\>
* #my-id: Selects \<p id="my-id"\> or \<a id="my-id"\>
* .my-class: Selects \<p class="my-class"\> and \<a class="my-class"\>
* img[src]: Selects \<img src="myimage.png"\> but not \<img\>
* a:hover: Selects \<a\>, but only when the mouse pointer is hovering over the link.

Anything in a CSS document between /* and */ is a CSS comment.

Most of the HTML elements on your page can be thought of as boxes sitting on top of each other.

CSS layout is based principally on the box model.

* padding, the space just around the content (e.g., around paragraph text)
* border, the solid line that sits just outside the padding
* margin, the space around the outside of the element

When you set two values on a property like *margin* or *padding*, the first value affects the element's top and bottom side, and the second value the left and right side.

When you set four values on a property like *margin* or *padding*, the values set top, right, bottom, left, in that order.

text-shadow

* The first pixel value sets the *horizontal* offset of the shadow from the text — how far it moves across: a negative value should move it to the left.
* The second pixel value sets the *vertical* offset of the shadow from the text — how far it moves down, in this example; a negative value should move it up.
* The third pixel value sets the *blur radius* of the shadow — a bigger value will mean a more blurry shadow.
* The fourth value sets the base color of the shadow.

### JavaScript basics

The reason we've put the *script* element near the bottom of the HTML file is that HTML is loaded by the browser in the order it appears in the file. If the JavaScript is loaded first and it is supposed to affect the HTML below it, it might not work, as the JavaScript would be loaded before the HTML it is supposed to work on. Therefore, putting JavaScript near the bottom of the HTML page is often the best strategy.

Mixing data types can lead to some strange results when performing calculations, so be careful that you are referring to your variables correctly, and getting the results you expect.

The name is stored inside *localStorage*, it persists after the site is closed down, keeping the personalized message there when you next open the site!

### Publishing your website

### How the web works

## HTML — Structuring the web

## CSS — Styling the web

## JavaScript — Dynamic client-side scripting

## Accessibility — Make the web usable by everyone

## Tools and testing

## Server-side website programming

## Further resources

### Common questions

#### How do you set up a local testing server?

Navigate to the directory that your web is inside, using the cd command.

Enter the command to start up the server in that directory:

    # On Mac and Linux
    python -m SimpleHTTPServer
    # On Windows and Mac
    python -m http.server

By default, this will run the contents of the directory on a local web server, on port 8000. You can go to this server by going to the URL localhost:8000 in your web browser.
