<!-- First topic: How to write an HTML Boilerplate -->
<!-- Link:  https://www.freecodecamp.org/news/basic-html5-template-boilerplate-code-example/ -->

# Example of HTML 5 boilerplate
Let's take a look at a basic example.

```html
 <!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>HTML 5 Boilerplate</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <script src="index.js"></script>
  </body>
</html>
```

# What is a doctype in HTML?

The first line in your HTML code should be the doctype declaration. A doctype tells the browser what version of HTML the page is written in.

```html
<!DOCTYPE html>
```
If you forget to include this line of code in your file, then some of the HTML 5 tags like

`<article>`, `< footer >`, and `<header>` may not be supported by the browser.

# What is the HTML root element?

The `<html>` tag is the top level element of the HTML file. You will nest the `<head>` and `<body>` tags inside of it.

```html 
<!DOCTYPE html>
<html lang="en">
  <head></head>
  <body></body>
</html>
``` 
The `lang` attribute inside the opening `<html>` tag sets the language for the page. It is also good to include it for accessibility reasons, because screen readers will know how to properly pronounce the text.

# What are head tags in HTML?

The `<head>` tags contain information that is processed by machines. Inside the `<head>` tags, you will nest metadata which is data that describes the document to the machine.

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>HTML 5 Boilerplate</title>
    <link rel="stylesheet" href="style.css">
</head>
```

# What is UTF-8 character encoding?
UTF-8 is the standard character encoding you should use in your web pages. This will usually be the first `<meta>` tag shown in the `<head>` element.

```html
<meta charset="UTF-8">
```

According to the [World Wide Web Consortium](https://www.w3.org/International/questions/qa-choosing-encodings),

> A Unicode-based encoding such as UTF-8 can support many languages and can accommodate pages and forms in any mixture of those languages. Its use also eliminates the need for server-side logic to individually determine the character encoding for each page served or each incoming form submission.

# What is the viewport meta tag in HTML?

This tag renders the width of the page to the width of the device's screen size. If you have a mobile device that is 600px wide, then the browser window will also be 600px wide.

The initial-scale controls the zoom level. The value of 1 for the initial-scale prevents the default zoom by browsers.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">`
```

# What does X-UA-Compatible mean?
This `<meta>` tag specifies the document mode for Internet Explorer. IE=edge is the highest supported mode.

```html
<meta http-equiv="X-UA-Compatible" content="ie=edge">
```

# What are HTML title tags?
The `<title>` tag is the title for the web page. This text is shown in the browser's title bar.

```html
<title>HTML 5 Boilerplate</title> 
```
>
#
![HTML 5 Boilerplate picture](https://www.freecodecamp.org/news/content/images/2021/07/Screen-Shot-2021-07-30-at-4.15.25-AM.png)