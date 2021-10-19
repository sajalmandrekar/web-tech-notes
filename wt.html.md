## HTML

<!DOCTYPE>

#### `<html> </html>` tag

__HTML Attributes:__

1. dir: direction of text ("ltr","rtl"), e.g. `<html dir="ltr"> ... </html>`
2. id
3. lang
4. version

#### `<head></head>` tag

__HEAD Attributes:__
1. style
2. title
3. dir, id, lang, ... etc
__Content:__
* title tag, base tag, ...etc

#### `<title> </title>` tag

* __Attribute:__ class, id, lang, style
* __Content:__ title of the web page

#### `<body></body>` tag

* __Attribute:__ bgcolor, background, leftmargin, topmargin, text, alink, class, id, lang, ..etc
* __Content:__ content to be displayed on web page, also includes various other tags

#### Hyperlinks

* `<a href="" target="_blank"> Click to open link </a>`
* href: destination of file e.g. href="dir/file.html"
* target: "_blank" means new tab or default is same tab
* setting hyperlink colors
    * `<body alink="" vlink="" link="">`
    * link: color of link not visited
    * vlink: color of link visited once
    * alink: color of active link 
* going to different section of page
    * e.g. `<a href="#SECTION_A"> Text </a>`
    * ... `<a name = SECTION_A> <h2>This is section A</h2></a>`

#### Forms
* `<form action="submit.html" method="get"> ... </form>`
* attribute:- action:which page to go when clicked submit, method: get or post
    * `<input type="text" name=""> Text </input>`
    * __atribute:__ name,size,maxlength,type:(button,checkbox,file,image,password,reset,submit,text,radio,hidden), align

#### Text area
* `<textarea cols="10" rows="20"> ... </textarea>`

#### Select and Options
* `<select> ... </select>`
    * `<optgroup label="Label name"> ... </optgroup>`
    * `<option value="val_name">Display value</option>`
    * `<option> may be under <optgroup> under <select>`
    * `<select> is used under a form`

#### paragraphs
- `<p></p>`: new lines before and after
- `<br />` to add new line in para
- __attribute:__ align:(left,center,right) !not suported in html5

#### images
* `<img>`
* __attribute:__ src: destination of file, alt:alternate text, title:"name appears when cursor hovered over image", heigth:"in % or px", width, border:" in px", align:(left,right,center)

* __example:__` <img src="" alt="" border="" title="">`
* __image as link:__ `<a href="web.html"> <img src="abc.jpg"> </a>`
* __image mapping:__

```
<img src="cat.jpg" usemap="#MyMap"> </img>
<map name = "MyMap">
<area shape="rect" title="rectangle" coords="0,0,82,126" href="lec2.html">
<area shape="circle" title="circle" coords="190,200,200" href="lec1.html">
```

#### tables

* `<table>` tag used to create a tables
* `<tr>` to create rows
* `<td>` tag to add values to coloumns
* __table attributes:__ border, align:(right,left,center)
* __td attribute:__ colspan, bgcolor(eg, "red")
* __rowspan__: `<th rowspan="4">name</th>` (4 denotes 3 rows are present already)