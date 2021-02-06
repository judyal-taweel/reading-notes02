# How the Web Works

When you visit a website, the web server hosting that site could be anywhere in the
world. In order for you to find the location of the web server, your browser will first connect
to a Domain Name System (DNS) server.

1. When you connect to the web, you do so via an Internet Service
Provider (ISP). You type a domain name or web address
into your browser to visit a site; for example: `google.com` .

1. Your computer contacts a network of servers called Domain Name System (DNS)
servers. These act like phone books; they tell your computer the IP address associated with
the requested domain name. An IP address is a number of up to 12 digits separated
by periods / full stops. Every device connected to the web has a unique IP address; it is
like the phone number for that computer.

1. The unique number that the DNS server returns to your computer allows your browser
to contact the web server that hosts the website you requested. A web server is a
computer that is constantly connected to the web, and is set up especially to send web pages to users.

1. The web server then sends the page you requested back to your web browser.


# HTML Describes the Structure of Pages

HTML has several semantic elements that define the different parts of a web page:
Header
`<header></header>`

<h1> headings should be used for main headings, followed by <h2> headings, then the less important <h3>, and so on.

Paragraphs
<p> </p>

A paragraph always starts on a new line, and is usually a block of text.

Links
<a href="#">This is a link</a>

![body](imgs/body.PNG)

You met the <body> element in the first example we created. Everything inside this element is
shown inside the main browser window.

Before the <body> element you will often see a <head> element. This contains information
about the page (rather than information that is shown within the main part of the browser
window that is highlighted in blue on the opposite page). You will usually find a <title>
element inside the `<head>` element.


# The Evolution of HTML

Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a
browser which version of HTML the page is using.

![DOCTYPE](imgs/doctype.PNG)

### Comments in HTML

`<!-- -->`
If you want to add a comment to your code that will not be visible in the user's browser, you
can add the text between these characters:
`<!-- comment goes here -->`

### ID Attribute

Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the
page. Its value should start with a letter or an underscore (not a number or any other character). It is important that no two elements on the same page
have the same value for their id attributes (otherwise the value is no longer unique).

### Class Attribute

Every HTML element can also carry a class attribute. Sometimes, rather than uniquely identifying one element within
a document, you will want a way to identify several elements as being different from the other elements on the page.

### Block Elements

Examples of block elements are
`<h1>`, `<p>`, `<ul>`, and `<li>`

### Inline Elements

Examples of inline elements are
`<a>`, `<b>`, `<em>`, and `<img>`.

### Grouping Text & Elements In a Block

The `<div>` element allows you to group a set of elements together in one block-level box.


### IFrames

An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term
iframe is an abbreviation of inline frame.

![IFrame](imgs/ifram.PNG)


### Escape Characters

![Escape](escape.PNG)

# Traditional HTML Layouts

For a long time, web page authors used <div> elements to group together related elements on the page (such as the elements that form a
header, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the <div> element in the structure of the page.

![Layout](imgs/layout.PNG)

### Headers & Footers

`<header> <footer>`

The <header> and <footer> elements can be used for:
- The main header or footer that appears at the top or bottom of every page on the site.

- A header or footer for an individual <article> or <section> within the page.

### Navigation

The `<nav>` element is used to contain the major navigational blocks on the site such as the primary site navigation.

### Articles

`<article>`

### Sections

`<section>`


# Process & Design

- Who is the Site For?
- Why People Visit Your Website?
- What Your Visitors are Trying to Achieve?
- What Information Your Visitors Need?
- How Often People Will Visit Your Site?

### Site Maps

The aim is to create a diagram of the pages that will be used to structure the site. This is
known as a site map and it will show how those pages can be grouped.

![map](imgs/map.PNG)

### WireFrames

A wireframe is a simple sketch of the key information that needs to go on each page of a
site. It shows the hierarchy of the information and how much space it might require.

![wireframe](imgs/wireframe.PNG)

- You can differentiate between pieces of information using size, color, and style. 


- You can use grouping and similarity to help simplify the information you present.



# Java Script

![java1](imgs/java1.PNG)

![java2](imgs/java2.PNG)

![java3](imgs/java.PNG)