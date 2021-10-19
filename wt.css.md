# CSS - cascading style sheets

* format: selector{property:value;}
* advantages of css
    - write once, use multiple times
    - easy maintainence
    - simple less code
* disadvantages - compatibility

### basic syntax:
```
<HEAD>

<STYLE TYPE="text/css“>

tagname {styleattribute : value; }

</STYLE>

</HEAD>
```

### css in html:
**Adding In-line style sheets**

1. inside head tag

    ```
    <head>
        <style> 
            h1{
                font-style:italic;
                color:#000090
            }
            h2{
            ...
            }
        </style>
    </head>
    ```

2. link to external css sheets
    * `<link> should be present inside <head></head>`
    * `<link rel="stylesheet" href="mystyle.css">`

3. inline style sheet added into middle of HTML
    * `<h2 style="color:red;font-size:+27pt">Heading</h2>`

### text attributes in css
* applies for p, h, body, etc
* font-size, font-style:(normal,italic,oblique), font-weight:(normal,bold,lighter,100,200,...), color:#HEX, background-color:#HEX, text-decoration:(underline,overline,blink), text-transform:(uppercase,capitalize), font-variant:(small-caps), font-family
* set background in body: `background: url();`

### grouping
* example:
```
h1,h2{
    color:blue;
}
```

### Class as selector
1. define a class in CSS:
    ```
    .myclass{
        color:cyan;
        font-size:15pt;
    }
    ```
2. `<p class="myclass"> Web tecnologies by prof. Teslin </p>`

### ID as selector
1. in css
    ```
    #uniqueId{ font-size:12pt; color:blue;}
    ```
2. `<div id="uniqueId"> ... </div>`
* note: id as selector is unique and only used once

### contextual selectors
* eg. h2 em{}
* `<h2>... <em>....</em>...</h2>`
* div p{} :The first selector matches all P elements that have a DIV among the ancestors.
* .red h1{} :The second selector matches all H1 elements that have an element of class red.

### positioning
* absolute positioning
    * property: value
        * position:absolute;
        * top: 5px; left:5px; z-index:3;
    * example:
    `<h2 style = "position : absolute; top : 5px; left : 5px; z-index:3"> Positioning Element </h2>`
* relative positioning
    * position: relative;
    * top: 10px; bottom:10px
    * eg: `.sub { position : relative; bottom : -1ex }`

### Background
* property:values
    * background-position:(bottom right,top left,...)
    * background-image:
    * background-repeat:(repeat,no-repeat)
    * background-attachment:(fixed,scroll)

### Element dimension
* set the dimaentions of an element
* width, height:(in %,cm,pt,px, ..etc)
