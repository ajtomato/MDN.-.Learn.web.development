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

### JavaScript basics

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
