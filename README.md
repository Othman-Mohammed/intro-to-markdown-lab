<!-- Part A -->
# Writing a Function in JavaScript

In JavaScript, functions are blocks of reusable code. They allow you to bundle functionality, make it more readable, and avoid repetition. Here's a brief tutorial on writing an arrow function in JavaScript.

## 1. Basic syntax
```JavaScript
consAt functionName = (params) => {
  // code to be executed
}
```

1. **const**: const should be used whenever a function expression is assigned to a variable.
2. **The function name**: The name you choose for the function.
3. **Parameters**: Optional comma separated parameters. This is the data passed into the function. If there are no parameters, the () is still required.
4. **The arrow syntax**: Indicates that this will be a function.
5. **The body**: The statements that make up the function itself. Surrounded by curly braces.

***Example***:
```JavaScript
const greet = (name) => {
  console.log("Hello, " + name + "!");
}
```
> Tip: Functions often perform actions, so naming with a verb can make it clear what the function does. Examples include fetchData( ), calculateArea( ), or printReport( ). 

## 2. Calling a function

To execute the function, you *call* or *invoke* it by using its name followed by parentheses.

***Example***:

`greet('Alice');` // Outputs: Hello, Alice!

## 3. Return values

Functions can process data input and output a value using the *return* keyword.

***Example***:

```JavaScript
const addNums = (numA, numB) => {
  return numA + numB
}

const total = addNums(2, 4);

console.log(total) // Expected value: 6 
```
<!-- This is a direct link -->
For more information on functions and how they are used in JS, check out the MDN docs. 
[Here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

![Adventure](https://images.unsplash.com/photo-1745949779026-f7fdd1470f8c?q=80&w=687&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)

<!-- Those are my notes just ignore them -->

<!-- [Google](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions) -->

<!-- This is a reference link -->
<!-- please [click me][x]

[x]: https://generalassembly.instructure.com/courses/907/assignments/23532?module_item_id=89427 -->


<!-- Summary -->
<!-- 
README file type is md (README.md)

ctrl + shift + v -> to have the preview readme view

# -> h1
## -> h2
### -> h3 and so on...

_text_ or *text* -> italic 
__text__ or **text** -> bold
___text___ or ***text*** -> bold and italic

For LISTS:
* -> filled bullet point 
tab+* -> bullet point under one bullet point (other ways are + and -)

for NUMBERS:
1. -> normal number 
tab+1. -> under 1 we will have another 1 (nested)

`code goes here` -> wrapping the inline code

```code goes here``` -> for multiline code (we can specify the name of the programming language)
e.g. ```HTML 
        code here 
     ```
[name](line goes here) -> for direct link

[name][nameX] then [nameX]: link -> for a reference link
e.g.  This is [a reference][example].

[example]: http://www.example.com/
Note: there must be one line gap between them

> -> this is to write a blockquote

Those are nested blockquotes
>
>>
>>>

![text](url) -> to add an image using url 
e.g. ![Computer with Code](https://images.unsplash.com/photo-1587620962725-abab7fe55159?auto=format&fit=crop&q=80&w=1631&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)
![text](path of the image) -> to add image using path 

| Syntax | Description |
| ------ | ----------- |      ->   To create a table
| Header | Title |
| Paragraph | Text | 

- [x] text 1 -> to create a task list (checked)
- [] text 2 -> to create a task list (unchecked)

~~text~~ -> to have strikethrough over the text (line on the text)

 -->


<!-- Part 2 Starts from here  -->

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