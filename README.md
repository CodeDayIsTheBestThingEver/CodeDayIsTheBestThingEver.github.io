# My New Year's Resolution App

This is the first in a series of apps that will help you build a website - an app where you can keep your friends, family, and audience up to date on whether or not you're achieving your New Year's Resolution goals. Not doing New Years resolutions? Choose any yes or no status, like "Is it too cold for Jenn to drink iced almond milk lattes?" 

This project relates to video 1 of 4 in the [Website Starter Kit](https://glitch.com/website-starter-kit) video series.

[![](https://cdn.glitch.com/6d561a98-036e-47a6-b152-a2a66a73d13e%2FjennPlay.png?1518516252256)](https://www.youtube.com/watch?v=xkenZ6bukEo)

Coding is challenging, but if you take it day by day and practice, you can build the app of your dreams in no time - and we at Glitch and in the community are here to help!

Here's the entire list of apps in this series:

* [intro to html](https://glitch.com/edit/#!/intro-to-html)
* [intro to css](https://glitch.com/edit/#!/intro-to-css)
* [intro to js](https://glitch.com/edit/#!/intro-to-js)
* [intro to node](https://glitch.com/edit/#!/intro-to-node)

## Here is a very short introduction to HTML

HTML stands for HyperText Markup Language. It is a language for adding content to a web page or app. The result of HTML is not pretty - most browsers default to using Times New Roman font and blue links  - but the ability to add content to a site that anyone on the Web can see is very powerful! After learning HTML, you can explore other languages that let you style the page and add dynamic features.

The first thing you usually see in an HTML document is the "doctype":

```
<!DOCTYPE html>
```

The doctype is a peculiar looking line that tells the browser that the code that comes after is HTML. Almost as peculiar is that the next thing you'll typically see is this:

```
<html>
```

HTML uses tags for sandwiching content, and we call them *elements*. For example, here is a paragraph element:

```
<p>This is a paragraph!</p>
```

The content starts with a `<p>` tag and ends with a `</p>` tag, so the browser knows where the paragraph starts and begins. Most HTML documents after the doctype starts with that `<html>` tag and ends with the `</html>` tag.

Within an HTML document, there is a "head" and "body" - the head holds info for the browser, the body holds the content that people looking at our site can see. This app and many you'll encounter are structured like this:

```
<!DOCTYPE html>
<html>
<head>
  <title>This is the title that shows on the tab of my browser</title>
</head>

<body>
  
  <p>Here is some content.</p>
  
</body>
</html>
```

White space doesn't matter in HTML beyond a single space between words in the content. The above example renders the same as the following, which has more whitespace:

```
<p>
  This is a paragraph!
</p>
```

Depending on your preferences, you may want more or less whitespace. Whatever helps you personally write the most readable and maintainable code is best!

Another way to make your code readable and maintainable is with comments:

```
<!-- this is a comment that you can only 
      see in the source code -->
<h1>This is a heading!</h1>
```

In the above snippet of code, there is a comment above an element. Anyone going to the site will only see the large heading, and anyone viewing the source code will see the comment and the heading. Comments are great for documenting what you're trying to do with the code. Heading tags (`<h1></h1>, <h2></h2>, ..., <h6></h6>`) are great for letting people know the headings of content - which is also useful to screenreaders and other tools reading the content.

Some elements don't have an ending tag and are *self-closing*, like for line breaks:

```
<br />
```

And there are some elements that need to give the browser more info to render them, and we give that info in the form of *attributes*. Attributes have a name and value:

```
<p id="introduction">This is a paragraph!</p>
```

The attribute above is called `id` and the value is `introduction`. We use attributes like `id` and `class` to select them in other languages like CSS and JavaScript. Some attributes are required for HTML, like in images:

```
<img src="example.png" alt="my example image" />
```

The above image element requires two attributes: `src` needs the source URL of the image, and `alt` needs the alternate text in case the user cannot see the image - like if they are using a screenreader or the images haven't loaded yet.

The true power of the Web is the ability to link to other pages. In order to make text become a link, we wrap that text in an `a` or "anchor" tag and give the url as an `href` attribute:

```
<a href="resolution.html">information about my new year's resolution</a>
```

## You know a little about HTML, but there is a lot more!

What's great about building for the Web in HTML is that there are a lot of resources. Googling what you're looking to do, or to look up a tag you don't recognize, is usually effective. I also highly recommend [MDN's HTML documentation](https://developer.mozilla.org/en-US/docs/Web/HTML), which includes info on these and other tags, along with beginner tutorials.

Probably the most fun way to dive into HTML is to just go for it - check out the files in this project and play around until it has the content you want it to have!

Tomorrow, we'll learn about Cascading Stylesheets (CSS) and how to use that language to make this app look nicer!


ヽ(๏∀๏ )ﾉ

## What files are in this project?

### assets

This is a folder where you can upload assets like images. This project has an illustration of books because the example resolution has to do with reading.

### ← README.md

This file you're reading is a file written in Markdown - which is shorthand for HTML. Developers use README files to describe what their project is, along with any other info they have for contributors and users. In this project's README.md file, we talk about what the project is and list the files that are within it. You should keep this file up to date as you add features and pages to your app!

### ← index.html

This is the home page of our app and it's written entirely in HTML. Keep it updated to let users know what the date is and if you're achieving your resolution goals or whatever status you want to track this month!

### ← about.html

This is another HTML page that we link to in `index.html`. In it, talk about what your resolution is and anything else that you want your audience to know about you and your goals this year!
