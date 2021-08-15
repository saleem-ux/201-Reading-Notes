## Structure
In all kinds of documents, structure is very important in helping
readers to understand the messages you are trying to convey
and to navigate around the document. So, in order to learn how
to write web pages, it is very important to understand how to
structure documents.
## Structuring Word Documents
The use of headings and
subheadings in any document
often reflects a hierarchy of
information. For example, a
document might start with
a large heading, followed by
an introduction or the most
important information.
This might be expanded upon
under subheadings lower down
on the page. When using a word
processor to create a document,
we separate out the text to give
it structure. Each topic might
have a new paragraph, and each
section can have a heading to
describe what it covers.
On the right, you can see a
simple document in Microsoft
Word. The different styles for
the document, such as different
levels of heading, are shown
in the drop down box. If you
regularly use Word, you might
have also used the formatting
toolbar or palette to do this.
## HTM L Describes the Structure of Pages
The HTML code (in blue) is made up of characters that live inside angled
brackets — these are called HTML elements. Elements are usually
made up of two tags: an opening tag and a closing tag. (The closing tag
has an extra forward slash in it.) Each HTML element tells the browser
something about the information that sits between its opening and
closing tags.
## Body, Head & Title
<body>
You met the <body> element
in the first example we created.
Everything inside this element is
shown inside the main browser
window.
<head>
Before the <body> element you
will often see a <head> element.
This contains information
about the page (rather than
information that is shown within
the main part of the browser
window that is highlighted in
blue on the opposite page).
You will usually find a <title>
element inside the <head>
element.
<title>
The contents of the <title>
element are either shown in the
top of the browser, above where
you usually type in the URL of
the page you want to visit, or
on the tab for that page (if your
browser uses tabs to allow you
to view multiple pages at the
same time).
## Comments in HTML
<!-- -->
If you want to add a comment
to your code that will not be
visible in the user's browser, you
can add the text between these
characters:
<!-- comment goes here -->
It is a good idea to add
comments to your code because,
no matter how familiar you
are with the page at the time
of writing it, when you come
back to it later (or if someone
else needs to look at the code),
comments will make it much
easier to understand.
Although comments are not
visible to users in the main
browser window, they can be
viewed by anyone who looks at
the source code behind the page.
On a long page you will often
see comments used to indicate
where sections of the page start
or end, and to pass on notes to
help anyone who is looking at
the code understand it.
Comments can also be used
around blocks of code to stop
that code from being displayed
in the browser. In the example on
the left, the email link has been
commented out.
## <meta>
The <meta> element lives
inside the <head> element and
contains information about that
web page.
It is not visible to users but
fulfills a number of purposes
such as telling search engines
about your page, who created
it, and whether or not it is time
sensitive. (If the page is time
sensitive, it can be set to expire.)
The <meta> element is an empty
element so it does not have a
closing tag. It uses attributes to
carry the information.
The most common attributes
are the name and content
attributes, which tend to be
used together. These attributes
specify properties of the entire
page. The value of the name
attribute is the property you
are setting, and the value of the
content attribute is the value
that you want to give to this
property.
In the first line of the example on
the opposite page, you can see a
<meta> element where the name
attribute indicates an intention
to specify a description for the
page. The content attribute is
where this description is actually
specified.
The value of the name attribute
can be anything you want it to
be. Some defined values for this
attribute that are commonly
used are:
description
This contains a description
of the page. This description
is commonly used by search
engines to understand what the
page is about and should be a
maximum of 155 characters.
Sometimes it is also displayed in
search engine results.
keywords
This contains a list of commaseparated
words that a user
might search on to find the page.
In practice, this no longer has
any noticeable effect on how
search engines index your site.
robots
This indicates whether search
engines should add this page
to their search results or not. A
value of noindex can be used if
this page should not be added. A
value of nofollow can be used
if search engines should add this
page in their results but not any
pages that it links to.
## New Html 5 Layout Elements
HTML5 introduces a new set of elements that allow you to divide up the
parts of a page. The names of these elements indicate the kind of content
you will find in them. They are still subject to change, but that has not
stopped many web page authors using them already.
Headers & Footers
<header> <footer>
Navigation
<nav> 
Articles
<article>
<aside>
<section>
Heading Groups
<hgroup>
Figures
<figure> <figcaption>
Sectioning El ements
<div>

