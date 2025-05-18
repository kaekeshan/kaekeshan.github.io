---
title: HTML
description: Hyper Text Markup Language
draft: false
tags: [seed, dev, note]
---

HTML helps to add structure to the webpage.  
current version of html = [html5](https://html.com/html5/)
The first file to parse will be ==index.html==.  
Common terms to note down are element (set of start, end tags and content in b/w).
For example: ```<p> This is a an example of element</p>```  
The start tag is : ```<TAG_NAME>```  
The end tag is : ```</TAG_NAME```
Concept of parent-child relation is important in HTML

#### Basic Structure of an HTML document

```html

<!DOCTYPE html> <!-- requried preamble -->
<html lang="en">
  <head> <!-- to delcare metadata, styles, script etc.. -->
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>My Website</title>
    <link rel="stylesheet" href="./style.css">
    <link rel="icon" href="./favicon.ico" type="image/x-icon">
  </head>
  <body> <!-- page content goes here -->
    <main>
        <h1>Welcome to My Website</h1>  
    </main>
    <script src="index.js"></script>
  </body>
</html>

```

### Definitions

HTML syntax information can be found [here](https://html.spec.whatwg.org/#syntax)

> [!tip] HTML indendation or linebreaks are not considered by Browser engines while rendering the webpage

#### Text Elements
- Comments : start with ```<!--``` and end with ```-->``` 
- Headings : ```<h1>``` to ```<h6>```, H1 > H2 .. > H6 
- Paragaraph : ```<p>```, in-line element
- Bold text : ```<b>``` : no semantic meaning, usage is discouraged  
            : ```<strong>``` : *recommended*
- Italics text : ```<i>``` : no sematic meaning, usage is dicouraged  
               : ```<em>``` : *recommended*
- List
    - Orderd list, start with ```<ol>``` and individual list items are enclosed within ```<li> ... </li>``` 
    - Unorderd list, start with ```<ul>``` and individual list items are enclosed within ```<li> ... </li>```



