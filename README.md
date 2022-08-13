https://devdocs.io/css/

1. HTML
``` sql

> Form:
 >> https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form
 >> Atrribute: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input
 
 <form>
   <label></label>
   <input></input>
 </form>
 
 <br>: break the line
 <hr>: create a horizontal line
 
 
 
 ```
 2. CSS - Cascaing Style Sheets
 ```ruby
 Good color for background: https://colorhunt.co/
 Border-style: https://developer.mozilla.org/en-US/docs/Web/CSS/border-style
 
> **Important order when different styles apply in the same html file:**
 >> In-line CSS
  >>> <body style="background-color: mintcream;">
 >> Internal CSS: insert at the head section
  >>> selector{prorperty: value;}
 >> External CSS: link at the head section as
  >>> <link rel="stylesheet" href="..." type="text/css">
  >>> In exteral css: .selector {property: value;}
  
> Syntax:
 >> selector {property: value;}
   >>> selector: who?
   >>> property: what?
   >>> value: how?
 
 > CSS reference: https://www.w3schools.com/cssref/
 
 > Diffrence betwween Class vs Id:
  >> .class {property: value;}  --- you can apply the same class in different positions
  >> #id {property:value;} --- you can only have a single id name in a whole page
  >> another selector:
   >>> img:hover {
    background-color: gold;
    } ---change the background color to gold when you point the mouse at the image
    
  > Favicons: favourite icons - icon inserted in the head
   >> https://www.favicon.cc/
  > Border styling:
   >> {border-width: 0px 10px 20px 30px}: top right bottom left
   >> {padding: 20px}: 20px of space from all edges of text to border
   >> {margin: 10px}: gaps between boxes
  
  > Display property:
   >> Block elements: headers, paragraphs, division, lists and list itenms, forms
   >> Inline elements: (span, images, anchors) it does not take the whole box like block
   >> **Inline-block element: combine**
   >> None: get rid of the element. we can use display: none or visibility: hidden
   
  > Positions:
   >> Static: go along with HTML rules and keep to the default HTML flow
   >> Relative: position that the element relative to it would have been position in static, doest not effect the flow of HTML
   >> Absolute: position the element relative to its parent, it effects the flow of HTML (the parent position has to be set as "relative")
   >> Fixed: position of element fixed even when we scoll the webpage

 > Font-family:
  >> Font stack:  https://www.cssfontstack.com/
  >> Goole font: https://fonts.google.com/?query=sacra&category=Handwriting
 
 > FLoating:
  >> float: left; --> float the image to the left and wrap the paragraph to the right
  >> clear: left; --> clear the floating of the text and return the element to where it should be without floating
  
   
   
   
 
 
 ```
 
