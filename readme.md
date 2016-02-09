# HTML Review

## Anatomy of HTML

```html
<div class="bio">
  <p style="color:red;">My name is Yon Yonson. I come from Wisconsin.</p>
  <img src="me.jpg" alt="Hello" />
</div>
```
- `<div class="bio">My name...</div>`: Element
- `<div>`, `</div>`: Tags
- `<div>`: Open-tag
- `</div>`: Close-tag
- `<img />`: Self-closing tag
- `class=""`: Attribute
- `style="color:red;"`: Inline styling. (**Bad**)
- `My name is Yon Yonson...`: Content

## Robin's Rules of HTML

1. Your HTML [**must always validate**](https://validator.w3.org/#validate_by_input).
- The **bare minimum** HTML for any webpage to validate is:
  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title>My Page</title>
    </head>
    <body>

    </body>
  </html>
  ```
- Elements have to nest.
  ```html
  Wrong: <tagOne><tagTwo></tagOne></tagTwo>
  Right: <tagOne><tagTwo></tagTwo></tagOne>
  ```
- Every open tag needs an end tag, except for `<img />` and `<link />` (and a few others).
- The first HTML file you make for any website should be `index.html`.
- Indentation is **really important** for readability (and employability).
  ```html
  <body>
  <main>
  <h1>This is wrong.</h1>
  </main>
  </body>

  <body>
    <main>
      <h1>This is right.</h1>
    </main>
  </body>
  ```
- Everything you *see on the page itself* goes in the `<body>`. Everything you *don't see on the page itself, but that somehow affects it* goes in the `<head>`.
  - The `head` generally includes `<title>` and any stylesheets and Javascript.
- Your `class` names should always be semantic:
  ```html
  <div class="centered">This is bad.</div>

  <div class="heading">This is good.</div>

  <header>This is better.</header>
  ```

## HTML You Are Not Allowed To Use Under Any Circumstances

This HTML is all stylistic -- that is, it has no semantic value.

```
<hr />
<small>
<big>
<b>
<i>
<u>
<center>
<font>
<blink>
<marquee>
color=""
border=""
bgcolor=""
width=""
height=""
```

## HTML You're Allowed To Use Only If You Know What You're Doing

This HTML is really easy for junior designers to abuse, and can make your code look poorly-written. Only break the rules if you know them!

```
<br />
<pre>
<code>
<kbd>
<iframe />
<table>
<style>*
style=""
```

> \* Use external stylesheets instead: `<link rel="stylesheet" href="myStylesheet.css" />`

## A More Detailed Walkthrough

https://github.com/ga-wdi-lessons/html-intro/blob/master/02_html.md#now-were-ready-to-learn-html

## You Do
  - [Fix This HTML](https://github.com/ga-wdi-exercises/html_fixit)
  - [Match the Tags](https://github.com/ga-wdi-exercises/html_tag_matching)
  - [Absolute and Relative Links](https://github.com/ga-wdi-exercises/dc_directory_tree)

## HTML "References" (Dictionaries)

- [W3Schools: More concise](http://www.w3schools.com/tags/tag_iframe.asp)
- [Mozilla: More detailed](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
