#UTF-8 charset
##Description
Some character encodings cannot directly represent all characters an author may want to include in a document, HTML offers other mechanisms, called character references, for referring to any character. As there are huge number of characters, representing meaning, around the globe, proper care must be taken when representing these in HTML documents.

If you have any non-ASCII text in your CSS file, for example non-ASCII characters in font names, in values of the content property, in selectors, etc., you need to be sure that the CSS parser knows how to transform the bytes into characters correctly, so that it understands your CSS code.

##Example
<meta charset="utf-8">
`"&amp;"` represents &
"&#97;" represents a
"&#35;" represents #
"&#169;" represents copyright symbol

##Recommended
* Define meta encoding in HTML file not in CSS file.
* Use the character special code to print in the html document, e.g write the code "&lt;" instead of ">" to avoid the conflict. 

##not Recommended
```html
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
```
* The reason to go with the short one is that it matches other instances where you might specify a character set in markup.
* Do not directy insert the special character, use charater code instead.

##Further references
[Getting Started](http://www.w3.org/International/getting-started/characters)
[Stackoverflow comparison between long and short form](http://stackoverflow.com/questions/4696499/meta-charset-utf-8-vs-meta-http-equiv-content-type)

