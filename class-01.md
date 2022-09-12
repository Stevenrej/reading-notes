# Reading Notes 1

## Getting Started:

### How the Web Works

How the web works provides a simplified view of what happens when you view a webpage in a web browser on your computer or phone.

This theory is not essential to writing web code in the short term, but before long you'll really start to benefit from understanding what's happening in the background.

Clients are the typical web user's internet-connected devices (for example, your computer connected to your Wi-Fi, or your phone connected to your mobile network) and web-accessing software available on those devices (usually a web browser like Firefox or Chrome).
Servers are computers that store webpages, sites, or apps. When a client device wants to access a webpage, a copy of the webpage is downloaded from the server onto the client machine to be displayed in the user's web browser.

Order in which component files are parsed
When browsers send requests to servers for HTML files, those HTML files often contain <link> elements referencing external CSS stylesheets and <script> elements referencing external JavaScript scripts. It's important to know the order in which those files are parsed by the browser as the browser loads the page:

The browser parses the HTML file first, and that leads to the browser recognizing any <link>-element references to external CSS stylesheets and any <script>-element references to scripts.
As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from <link> elements, and any JavaScript files it has found from <script> elements, and from those, then parses the CSS and JavaScript.
The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.
As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

### Website Design

First things first: planning
Before doing anything, you need some ideas. What should your website actually do? A website can do basically anything, but, for your first try, you should keep things simple. We'll start by creating a simple webpage with a heading, an image, and a few paragraphs.

To begin, you'll need to answer these questions:

What is your website about? Do you like dogs, New York, or Pac-Man?
What information are you presenting on the subject? Write a title and a few paragraphs and think of an image you'd like to show on your page.
What does your website look like, in simple high-level terms? What's the background color? What kind of font is appropriate: formal, cartoony, bold and loud, subtle?

 ### Javascript

 JavaScript is a programming language that adds interactivity to your website. This happens in games, in the behavior of responses when buttons are pressed or with data entry on forms; with dynamic styling; with animation, etc. This article helps you get started with JavaScript and furthers your understanding of what is possible.

JavaScript itself is relatively compact, yet very flexible. Developers have written a variety of tools on top of the core JavaScript language, unlocking a vast amount of functionality with minimum effort. These include:

Browser Application Programming Interfaces (APIs) built into web browsers, providing functionality such as dynamically creating HTML and setting CSS styles; collecting and manipulating a video stream from a user's webcam, or generating 3D graphics and audio samples.
Third-party APIs that allow developers to incorporate functionality in sites from other content providers, such as Twitter or Facebook.
Third-party frameworks and libraries that you can apply to HTML to accelerate the work of building sites and applications.

Variable	Explanation	Example
String	This is a sequence of text known as a string. To signify that the value is a string, enclose it in single quote marks.	let myVariable = 'Bob';
Number	This is a number. Numbers don't have quotes around them.	let myVariable = 10;
Boolean	This is a True/False value. The words true and false are special keywords that don't need quote marks.	let myVariable = true;
Array	This is a structure that allows you to store multiple values in a single reference.	let myVariable = [1,'Bob','Steve',10];
Refer to each member of the array like this:
myVariable[0], myVariable[1], etc.
Object	This can be anything. Everything in JavaScript is an object and can be stored in a variable. Keep this in mind as you learn.	let myVariable = document.querySelector('h1');
All of the above examples too.



1. Like a river the flow of data is beatiful and serene
The current is the browser picking up and pulling as it flows
gently accessing the DNS Server and bringing along what it allows
the water is cool and requests that website comes along with it
and like the leaves that flow all the rest of the data comes with too
Packets flow in such as all life runs through a river
and Just as a person walks by and sees the beauty of it all come together
The river assembles all and put on a display of what it carries
Under the water not all is known like how most do not fully understand
How rivers and data can be the most gorgeous of all 

2. The browser goes to the DNS Server and find the real address of the website
It then sends a HTTP request asking for a copy of the website
If server approves the request the server send a 200 OK message and starts sending poackets of information
the browser then assembles the chunks into a full webpage
The HTML is parsed first and looks for a <link> for CSS and <script> for Javascript
If any are found the server request that information and it is then sent back to the browser
The browser generate an in memory DOM Tree from the html as well as a CSSOM structure
The javascript is read, compiled and excuted 

3. You can find images in such places as google images but most have copyright on them so it is better to look for a place that offers free images with no copyright on them. Any of these found can be inserted in your webpage

4. a string is (let variable = '10')
while a number is (let varible = 10)

5. Varible are important becasue they store values 






Introduction to HTML

What is HTML?
HTML (HyperText Markup Language) is a markup language that tells web browsers how to structure the web pages you visit. It can be as complicated or as simple as the web developer wants it to be. HTML consists of a series of elements, which you use to enclose, wrap, or mark up different parts of content to make it appear or act in a certain way. The enclosing tags can make content into a hyperlink to connect to another page, italicize words, and so on.

The element is the opening tag, followed by content, followed by the closing tag.

Nesting elements
Elements can be placed within other elements. This is called nesting. If we wanted to state that our cat is very grumpy, we could wrap the word very in a <strong> element, which means that the word is to have strong(er) text formatting

Empty elements
Not all elements follow the pattern of an opening tag, content, and a closing tag. Some elements consist of a single tag, which is typically used to insert/embed something in the document. For example, the <img> element embeds an image file onto a page:

<img src="https://raw.githubusercontent.com/mdn/beginner-html-site/gh-pages/images/firefox-icon.png">

Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

An attribute should have:

A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)
The attribute name, followed by an equal sign.
An attribute value, wrapped with opening and closing quote marks.

header:
Usually a big strip across the top with a big heading, logo, and perhaps a tagline. This usually stays the same from one webpage to another.

navigation bar:
Links to the site's main sections; usually represented by menu buttons, links, or tabs. Like the header, this content usually remains consistent from one webpage to another — having inconsistent navigation on your website will just lead to confused, frustrated users. Many web designers consider the navigation bar to be part of the header rather than an individual component, but that's not a requirement; in fact, some also argue that having the two separate is better for accessibility, as screen readers can read the two features better if they are separate.

main content:
A big area in the center that contains most of the unique content of a given webpage, for example, the video you want to watch, or the main story you're reading, or the map you want to view, or the news headlines, etc. This is the one part of the website that definitely will vary from page to page!

sidebar:
Some peripheral info, links, quotes, ads, etc. Usually, this is contextual to what is contained in the main content (for example on a news article page, the sidebar might contain the author's bio, or links to related articles) but there are also cases where you'll find some recurring elements like a secondary navigation system.

footer:
A strip across the bottom of the page that generally contains fine print, copyright notices, or contact info. It's a place to put common information (like the header) but usually, that information is not critical or secondary to the website itself. The footer is also sometimes used for SEO purposes, by providing links for quick access to popular content.

The head of an HTML document is the part that is not displayed in the web browser when the page is loaded. It contains information such as the page <title>, links to CSS (if you choose to style your HTML content with CSS), links to custom favicons, and other metadata (data about the HTML, such as the author, and important keywords that describe the document). Web browsers use information contained in the head to render the HTML document correctly. In this article we'll cover all of the above and more, in order to give you a good basis for working with markup.

Other types of metadata
As you travel around the web, you'll find other types of metadata, too. A lot of the features you'll see on websites are proprietary creations, designed to provide certain sites (such as social networking sites) with specific pieces of information they can use.

For example, Open Graph Data is a metadata protocol that Facebook invented to provide richer metadata for websites. In the MDN Web Docs sourcecode, you'll find this:

<meta property="og:image" content="https://developer.mozilla.org/static/img/opengraph-logo.png">
<meta property="og:description" content="The Mozilla Developer Network (MDN) provides
information about Open Web technologies including HTML, CSS, and APIs for both Web sites
and HTML Apps. It also documents Mozilla products, like Firefox OS.">
<meta property="og:title" content="Mozilla Developer Network">
Copy to Clipboard
One effect of this is that when you link to MDN Web Docs on Facebook, the link appears along with an image and description: a richer experience for users.







1. HTML attributes are special words used inside the opening tag to control the element's behavior


2. In an html element there is an opening tag then the content followed by the closing tag, The entirity of that is the element 

3. an <arcticle> tag enlcoses a block of content that is fine on its own and does not need to be a part of the rest of the page while the <section> tag is for grouping a part of the page that is a piece of functionality 

4. header: <header>.
navigation bar: <nav>.
main content: <main>, with various content subsections represented by <article>, <section>, and <div> elements.
sidebar: <aside>; often placed inside <main>.
footer: <footer>.

5. Using metadata boosts your SEO efforts because it's written in the search engine's language

6. it is used to specify character set, page description, keywords, author of the document, and viewport settings


Miscellaneous

How to start to design a Website.

1.  You need to define what your goals are for the website.

2. What exactly do I want to accomplish?

Semantics

1.  It is because it does not have a semantic value 

2. Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
Screen readers can use it as a signpost to help visually impaired users navigate a page
Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
Suggests to the developer the type of data that will be populated
Semantic naming mirrors proper custom element/component naming

What is Javascript?

1. Store useful values inside variables. In the above example for instance, we ask for a new name to be entered then store that name in a variable called name.
Operations on pieces of text (known as "strings" in programming). In the above example we take the string "Player 1: " and join it to the name variable to create the complete text label, e.g. "Player 1: Chris".
Running code in response to certain events occurring on a web page. We used a click event in our example above to detect when the label is clicked and then run the code that updates the text label.

2. Using a <scipt> tag in your html to link it to your html page





## THINGS I WANT TO KNOW MORE ABOUT

I would really like to learn more about seo. ifle these articles gave a good indication of what is going on with SEO and meta data but would like to get more in depth with it







 [Back To 201 Notes](https://stevenrej.github.io/reading-notes/readingnotes201main)
