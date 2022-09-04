**Reference Link**
<p>
<a href ="https://dribbble.com/">Dribble</a><br>
<a href ="https://devdocs.io/css/">Developent DOCS</a><br>
 <a href="https://www.figma.com/files/recent?fuid=1140292514495248365">Wireframe Website</a><br>
</p>

**1. HTML**
<details><summary>Collapse</summary><p>

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
 
 </p>
 </details>
 
**2. CSS - Cascaing Style Sheets**
 <details><summary>Collapse</summary><p>
 
 ```ruby
 Good color for background: https://colorhunt.co/
 Border-style: https://developer.mozilla.org/en-US/docs/Web/CSS/border-style
 Button Generator: https://css3buttongenerator.com/
 Challenge: https://www.frontendmentor.io/
 
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
 
 > Media Querry Breakpoint:
 >> @media (min-width:750px) and (max-width:1028px) { //change something } : set up the change in responsive breakpoints webpage

 > Code regactoring:
  >> 1. Readability
  >> 2. Modularity
  >> 3. Efficiency
  >> 4. Length
 
 > Combine selectors:
  >> .selector1, .selector2 {}: apply to all selectors appear
  >> #id .class {}: select class that has parents as #id
  >> .class1.class2 {} :select element that has 2 classes

> Flexbox:
 >> .container {
  >>> Display: flex;
  >>> justify-content: space-between / center; - align items across the main axis. Not changing the width of the items
  >>> align-items: center; align items across the corss axis.
  >>>  gap: 8px: add space between flex items, similar to adding a margin to the items
  }
  
 >> .item {
  >>> Flex: 1  1 auto;
  >>> Flex-direction: column / row;
 } 

 ```
 </p></details>
 
**3. Boostrap -- Front-end Library**
Install bootstrap in HTML:
 <details><summary>Link install into HTML CSS</summary>https://getbootstrap.com/docs/5.2/getting-started/download/
  </details>
 <a href="https://getbootstrap.com/docs/5.2/components/navbar/">navbar</a><br>
 <a href="https://getbootstrap.com/docs/5.2/layout/grid/">Grid System</a><br>
 <a href="https://getbootstrap.com/docs/5.2/layout/containers/">Container</a><br>
 <a href ='https://getbootstrap.com/docs/5.2/components/carousel/'>Carousel</a><br>
 
 <details><summary>Collapse</summary><p>
 
 ```ruby
> <Navbar>: 
 >> .navbar and .navbar-expand are required for responsive collapsing
 >> .bg-dark: for dark background color
 >> .navbar-dark: dark color for navbar
 >> .navbar-brand: for company, product, project name
 >> navbar-toggler: left aligned by default,
 
 > Grid
  >> Responsive layout breakpoints: lg (Laptop), md (tablet), sm (phone) 
 
 > .Container:
  >> max-width: set at each responsive breakpoint
  >> container-{breakpoint}: which is width:100% until the specified breakpoint
  >> container-fluid: which is 100% width at all breakpoints
   >>> .container-fluid {
        padding: 3% 15% !important
        }
 > Carousel: slideshow components that cycling through elements
   >> .active class needs to be added to one of the slides - otherwise, carousel wont be visible
   >> Set the unique id on the .carousel for optional controls
   >> Control and indicator elements must have a "data-bs-target" attribute (or href for links) that matches the id on the .carousel
   
 > Card: provide a flexible and extensible content container with multiple variants and options
   >> Cards have no fixed width to start, so they'll natually fill the full width of its parent element. Could be customized with "sizing options"
 
   
 ```
 </p></details>
 
 **4. Web Design**
  <details><summary>Collapse</summary><p>
 
 ```ruby
 > Color Theory:
  >> Moods: 
   >> Red: love, enerygy, intensity
   >> Yellow: Joy, Intellect, Attention
   >> Green: Freshness, safety, growth
   >> Blue: Stability, trust, serenity
   >> Purple: Royalty, Weath, femiminity
 
 
 ```
 </p></details>
 
  **5. JavaScript**
  <details><summary>Collapse</summary><p>
 
 ```ruby
> BASIC:
 >> word.length: count the length of a string
 >> word.slice(a,b): slice the string from a to b
 >> word.toUpperCase() / WORD.toLowerCase(): WORD / word
 >> text1.concat(text2) : text1text2
 >> modulo: let 9 % 6 : = 3. Take the remaining of the division 
 >> x ++ : x = x + 1 : increment
 >> x += 2: the increment is 2 instead of 1 by default
 >> Math.power(3,2) : 3^2 = 9
 >> Math.round(3.5) = 6: round to the nearest whole number
 >> Math.random(): generate random 16 decimal number from 0 - 0.999999999999999
 >> Control Flow: 
  >>> if (track === "clear") {
   goStraight ();
   } else {
   turnRight();
   }
   
> Advance:
 >> Comparator:
  >>> ==: equal to (only content) such as 1 = "1"
  >>> ===: stickly equal to
  >>> && : and
  >>> ||: or
  >>> !: not
 >> Arrays: names = [name0, name1, name2, name3, etc.];
  >>> names.length; :count length of arrays
  >>> names.includes (name3): TRUE
  >>> names.push(name6);: add an element to the end of the array
  >>> name.pop: remove the last item from the array
 
 >> While loops: while (something is true) {//Do something}
  >> while (i < 2) {
     console.log(i)
     i++ ; 
     }
 >> For loops: for (i = 0; i < 2; i++) { // Do something}
  >> i = 0 : start
  >> i < 2: end
  >> i++: change step
 
> DOM: Document Object Model
 >> Get property: button (.innerHTML, .style, .firstChild)
 >> Set property:
 >> Call method: button (.click(), .appendChild(), .setAttribute())
 >> Document.querrySelector("button").click();
 
 >> getElementsByTagName("li")[2].style.color = "purple" : change the color of the item has index of 2 to purple
 >> getElementsbyClassName("btn"): select the elements by class
 >> getElementById("button"): the Element in this method is single, because there is no 2 elements have the same ID
 >> querrySelector("h1 / #title / .btn"): we can select whatever elements we want by putting the sign at front like CSS. We can combine the selectors as well (like CSS)
 >> querrySelectorAll ("#list .item") : select all the elements that satisfy the querry
 
 >> DOM style object: how to apply different style to objects instead of CSS
 >> document.querySelector("button").classList: add / remove / toggle ("invisible");
 >> .innerHTML vs .textcontent: the .innerHTML can add everything inside the elements like <strong>, <em> but .textcontent only change the content
 >> attributes: everything that goes in the tag name are attributes (class, href, type, src are all attributes)
  >>> document.querySelector("a").attributes;
  >>> .querySelector("a").getAttributes("href");: www.google.com
  >>> .querySelector("a").setAttributes("href", "www.bing.com");
 
>> .addEventListener(): set up a function that will be called whenever the specified event is delivered to the target.
 >>> Syntax: .addEventListener(type, listener, (options / useCapture));
 >>> "click": click the mouse on the button
 >>> "pressdown": press the keyboard button

>> Javascript Object: 
 >>> dictionary: varible {key1: dict1, key2: dict2, key3: dict3, ....}
 >>> variable.key1 = dict1
 
>> Construction function: the name of the function has be capitalized to differentiate with other functions
 >>> function BellBoy (name, age, workPermit, languages) {
 this.name = name;
 this.age = age;
 this.workPermit = workPermit;
 this.languages = languages;
 this.moveSuitcase = function () {alert("May I take your suitcase?");}
 }
 >>> let bellBoy1 = new BellBoy("Timmy", 19, true, ["French", "English"]);
 
>> Switch statement:
 >>> switch (expression) {
      case expression:
      
        break;  
      default:
      
 }
 ```
 </p></details>
