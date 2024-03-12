# Create a Link Using the href Attribute

## Learning Goals

- Write an `a` tag to create a link

## Introduction

We've got our HTML tags, and we've got our HTML tag attributes. How do we use
them together? We can figure it out by exploring the `a` tag and creating a
link.

## Getting Started

**Fork and clone** this lesson into your local environment. Navigate into its
directory in the terminal, then run `code .` to open the files in Visual Studio
Code.

## Write an `a` Tag to Create a Link

Open `index.html` in your text editor. Add an `a` tag with the inner text (the
text between the `<a>` tag and the `</a>` tag) of `Flatiron School` anywhere in
the file. Then set the `href` attribute of your new link element to
`https://flatironschool.com`.

Check your progress by running `npm test`. Failing tests will provide helpful
error messages that you can use to debug your code — read them closely for
hints!

Don't forget to open the `index.html` file in your browser so you can see the
changes as you go.

## Conclusion

Here we saw how an attribute helps the `a` tag do its job, which is to link to
another location. Now we can go on to explore some additional HTML tags.

## Resources

- [Mozilla Developer Network: HTML `<a>` Tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a)

###Next Lab

#HTML Lists, Images and Links
##Learning Goals
-Identify ordered, unordered and definition lists
-Identify images
-Identify links
-Identify HTML validation tools

##Introduction
You might be wondering what else is available to use to build out full webpages now that you are more familiar with the basics of HTML. How do you display an image? How do you add a formatted list of topics? How do you link page elements beyond text? Now you're ready to explore these fundamental tools. Here's a high-level overview before you dive into practicing with the labs.

##Identify Ordered, Unordered and Definition Lists
When we want to present a list of items in a clear, readable format, we turn to the HTML unordered list, represented by the ul tag.

<ul>
  <li>One item</li>
  <li>Another item</li>
</ul>
Here is how the HTML above looks when rendered in the browser:

One item
Another item
If it's important to distinguish a particular order of the items (as for a recipe or ranking), we use an ordered list, or the ol tag.

<ol>
  <li>First item</li>
  <li>Second item</li>
</ol>
Here is how the HTML above looks when rendered in the browser:

First item
Second item
Notice the nesting of our items within the lists. Each li is a list item contained in the larger ul or ol container.

Another type of list we can use is a definition list, which defines specific types of items.

<dl>
  <dt>First term</dt>
  <dd>Term definition</dd>
</dl>
Here is how the HTML above looks when rendered in the browser:

First term
Term definition
Identify Images
To include an image in our page, we use an img tag.

<img
  src="https://via.placeholder.com/800x600.png"
  alt="Alternative Text"
  title="Display Title"
  width="800"
  height="600"
/>
There are two notable things about the img tag: The first is that it does not have a closing tag. The image tag closes itself. Secondly, it handles a lot of attributes. Attributes are special keywords used on the tag to control the element's behavior, or provide additional information about the HTML element.

The alt attribute provides descriptive text the browser can display if it can't find the image file. The browser can also display the title text to give the user more information about the image. The width and height attributes define the size of the image that shows up in the browser.

Here is how the image element above looks when rendered in the browser:

Alternative Text

Identify Links
You might be familiar with basic link structure already, but here are other ways we can use them.

Beginning with a standard text hyperlink, we can wrap other elements inside of them.

<a href="http://example.com/">This is a link</a>
Here is how the HTML above looks when rendered in the browser:

This is a linkLinks to an external site.

What if we want to link an image instead of text? We can replace the text within the a tags with our image tag.

<a href="http://example.com/">
  <img src="https://via.placeholder.com/800x600.png" alt="Alternative Text" />
</a>
Here is how the HTML above looks when rendered in the browser:

Alternative Text

What about a link that will direct to an email address?

<a href="mailto:webmaster@example.com">Send an email</a>
Here is how the HTML above looks when rendered in the browser:

Send an email

Sometimes we might want to link to a specific location on the same webpage. We can then target an element that we identified or classified earlier.

<p id="tips">Useful Tips Section</p>
<a href="#tips">Jump to the Useful Tips Section</a>
Here is how the HTML above looks when rendered in the browser:

Useful Tips Section

Jump to the Useful Tips Section

When considering what location links point to, you will choose between relative or absolute links. A relative link directs to content within the same website.

<a href="about.html">This is a relative URL link</a>
Here is how the HTML above looks when rendered in the browser:

This is a relative URL link

An absolute link, on the other hand, links to external content and requires a fully defined URL path. This is likely the type of link you see most often.

<a href="http://example.com/">This is an absolute URL link</a>
Here is how the HTML above looks when rendered in the browser:

This is an absolute URL linkLinks to an external site.

Identify HTML validation tools
An HTML validator is used to check HTML markup elements for syntax errors. Syntax errors, such as open tags, extra spaces, or forgotten quotation marks, can cause a web page to look drastically different than the creator intended, or render correctly in one browser, but not in another.

It's easy to forget a closing HTML tag or miss a piece of punctuation when writing HTML. Fortunately, we have a tool that will check our markup for us and point out any errors. To validate our HTML, we can use the W3 HTML validatorLinks to an external site..

Conclusion
Now that you've taken a first look at these new HTML elements, you'll be better prepared to practice them in labs, where you'll learn more about each one and how to use it effectively.
