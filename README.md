#UTF-8 charset
UTF-8 is a variable-width encoding that can represent every character in the Unicode character set. It was designed for backward compatibility with ASCII and to avoid the complications of endianness and byte order marks in UTF-16 and UTF-32. UTF-8 has become the dominant character encoding for the World Wide Web, accounting for more than half of all Web pages. 

If you have any non-ASCII text in your CSS file, for example non-ASCII characters in font names, in values of the content property, in selectors, etc., you need to be sure that the CSS parser knows how to transform the bytes into characters correctly, so that it understands your CSS code.

##Example
<meta charset="utf-8">

##Recommended
define meta encoding in HTML file not in CSS file

##not Recommended
```html
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
```
The reason to go with the short one is that it matches other instances where you might specify a character set in markup.

##Further references
[Getting Started](http://www.w3.org/International/getting-started/characters)
[Stackoverflow comparison between long and short form](http://stackoverflow.com/questions/4696499/meta-charset-utf-8-vs-meta-http-equiv-content-type)

