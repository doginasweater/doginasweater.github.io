---
short_name: step-2
name: Your First Page
step_number: 2
title: Your First Page
---

## Your first page

A website requires, at minimum, two things:

1. A server
2. A client

A server is nothing more than a special program able to respond to http requests. A client is nothing more than something able to deal with http responses.
`http` is short for hypertext transfer protocol, which is a really fancy way of saying "rigidly structured, well-defined way for things to communicate."
Think of it as a language of the internet.

You use http clients all the time. Almost every app you use communicates with the internet over http. But the most common one of all is your browser. A browser is just an http client that knows how to render web sites.

Believe it or not, a website is actually a special case of an http request. It's a request where the response is comprised of `html`, or hypertext markup language. `html` describes the structure of a web page, like a skeleton. You can build a website entirely out of `html`, but like most things comprised solely of bones, it won't be very appealing.

`html` has some strict rules as to how it is structured, and a limited set of tags to build a page. A tag looks like this:

```html
<!-- this is a comment -->
<div>this is a div</div>
<p class="hello">this is a paragraph with class hello</p>
<span id="my-span">this is a span with id my-span</span>
<a href="#">i'm a link</a>
```

It is comprised of the opening tag (`<div>`, `<p>`, `<span>` in the examples), optional properties or attributes (`id`, `class`, and `href` in the examples), content (what's in between the closing `>` and opening `<`), and a closing tag (`</div>`, `</p>`, `</span>`, `</a>`). Some tags, like `<img />` (images) and `<input />` are self-closing, so they don't require a closing tag, but they are required to end with `/>` instead of just the usual `>`.

A properly structured html file has a few required tags:

```html
<!DOCTYPE html>
<html>
  <head></head>
  <body></body>
</html>
```

`<!DOCTYPE html>`

The very first line will be the doctype. There are a few possible doctypes, but this one tells the browser/client/parser/consumer that what follows is html, or, more pedantically, something more modern than HTML 4.01. There's a group called the W3C (World Wide Web Consortium) that creates the html standard. They used to version it, but decided to stop around 5 when browser vendors started making new features faster than they could standardize them. For a while, we used the term `html5`, but that's fallen out of style. Sometimes you'll hear it when someone is specifically trying to refer to modern html.

`<html>`

The html tag, unsurprisingly, says "this is the start of the html"

`<head>`

The head, short for header, talks about the page that's about to be displayed. Information in the `<head>` won't be shown to the user, but it's useful for telling the browser that there's some extra information. You can put in a `<title>` to give the page a title (what's shown in the tab), link to your css, describe the language of the page, optinally load scripts, etc. There's a small list of tags that are valid in the `<head>`. Most of them are not allowed in the body.

`<body>`

The body is where the page content goes. Most of the work you do will be in the body. The list of tags you can use in the `<body>` is *much* larger than the `<head>`.

## Common tags

- `<p>` - defines a paragraph. Useful for displaying text.
- `<b>` and `<strong>` - makes text **bold**
- `<i>` and `<em>` - makes text *italic*
- `<a href="">link text</a>` - defines a link. The address goes inside the `href` attribute, and the link text goes in between the tags.
- `<ul>` - unordered list. Also known as a bulleted list.
- `<ol>` - ordered list. Displays a list with numbers.
- `<hr />` - horizontal rule. Makes a horizontal line.

This is by no means a comprehensive list. I recommend you look at [the mozilla developer network docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element) for more information.

## Exercise

Let's put our new knowledge to use! You can open any html file in a browser, so we're going to make one now.

1. Open visual studio code and create a new file. 
2. Down at the bottom right, click where it says Plain Text. A menu will pop up. Select HTML.
3. Put in the required tags.
4. Give the page a title of "My First Page"
5. Put the text "Hello, world!" in a `<p>` tag in the body.
6. Save the file.
7. Open the file in the browser of your choice.
8. You should see the text "Hello, world!"

Congratulations! You've officially written your first html page.