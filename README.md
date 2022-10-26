<details><summary>FRONT-END</summary>
**Reference Link**
<p>
<a href ="https://dribbble.com/">Dribble</a><br>
 <a href="https://www.figma.com/files/recent?fuid=1140292514495248365">Wireframe Website</a><br>
</p>

**1. HTML**
<details><summary>Collapse</summary><p>

``` python
>Table: 
>> thead
 >> tr: table row
  >>> <th rowspan = "2" colspan = "2">: table header
 >> /tr
>> /thead
>> tbody
  >>> td: table data - single cell
  >>> td: table data - single cell
>> /tbody
>> tfoot 

> Form:
 >> https://developer.mozilla.org/en-US/docs/Web/HTML/Element/form
 >> Atrribute: https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input
 
 <form action = "/" method="post" onsubmit="runMe(); return false">
  >> action: WHERE the form data should be sent
  >> method: which HTTP method should be used
   <label for = "{input ID}"></label>
   <input type = "{text / password / email / range / color / number / time / file / checkbox / radio / select} name={input name}"></input>
      >> input name: is used to link with button to send data to the server
      >> radio: all the connected radios must have the same "name" and different "value"
      >> checkbox could be used attribute "checked" as default
   <button type="{button / submit}">Submit</button>
      >> <select name="" id=""><option value=""></option></select>
      >> <range name="" id="" min="" max="" step=""
  >> <textarea name="" row="10" cols="30">
 </form>
 - Form validation: required / minlength-maxlength (for string) / min-max(for number) / 
 
<video | audio controls> 
   <source src = "....">
</video | audio>

<ifram src = "...." width = "500px" height = "700px" framebody = "0"></iframe> // add another website to our website like google maps, youtube

<small>Copyright &copy 2022. All rights reserved.</small> // create a copyright

  
 <br>: break the line
 <hr>: create a horizontal line
 
 ```
 </details>
 
**2. CSS - Cascaing Style Sheets**
 <details><summary>Collapse</summary><p>
 
 ```ruby
 Good color for background: https://colorhunt.co/
 Border-style: https://developer.mozilla.org/en-US/docs/Web/CSS/border-style
 Button Generator: https://css3buttongenerator.com/
 Challenge: https://www.frontendmentor.io/
    
> Pseudo:
 >> Classes: hover, checked, active, nth-child, nth-of-type
  >>> img:hover {
    background-color: gold;
    } ---change the background color to gold when you point the mouse at the image
 >> Element:: after / before / first-letter / first-line / selection
  >>> ::selection: change the style of selected element
  
    
  > Favicons: favourite icons - icon inserted in the head
   >> https://www.favicon.cc/
  > Border styling:
   >> {border-width: 0px 10px 20px 30px}: top right bottom left
   >> {padding: 20px}: 20px of space from all edges of text to border
   >> {margin: 10px}: gaps between boxes
 
 - Box Model:
 > Border: border-width / border-color / border-style
  >> box-sizing: boder-box; -- set the border-box as box-size
  >> box-style: solid / dotted / inset / dashed / double;
  >> border: 10px double #000; - shorthand for setting border
  
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
 
 > Display property:
   >> Block elements: take up the whole line
   >> Inline elements: width and height are ignored. Padding could be added but it does not take any space. It does not push other elements away. 
   >> Inline-block element: width, height, padding and margin could be changed respectively
   >> None: get rid of the element. we can use display: none or visibility: hidden
   
  > Positions:
   >> Static: go along with HTML rules and keep to the default HTML flow
   >> Relative: position that the element relative to it would have been position in static, doest not effect the flow of HTML
   >> Absolute: position the element relative to its parent, it effects the flow of HTML (the parent position has to be set as "relative"). There is no space created for the element
   >> Fixed: position of element fixed even when we scoll the webpage
   >> sticky: it go along with the page when we scoll down but it does not stick on the top (not fixed at first then fixed later)
   
 > Relative units:
  >> width: 50%: set the width 50% of its parent
  >> em: 1em = font size of the parent. 2em = 2* font-size of the parent. For other properties like padding, margin, em is refered to the font-size itself
  >> rem: relative to the root element's font-size.
  
 > Font-family:
  >> Font stack:  https://www.cssfontstack.com/
  >> Goole font: https://fonts.google.com/?query=sacra&category=Handwriting
 
 > FLoating:
  >> float: left; --> float the image to the left and wrap the paragraph to the right
  >> clear: left; --> clear the floating of the text and return the element to where it should be without floating
 
 > Media Querry Breakpoint:
 >> @media (min-width:750px) and (max-width:1028px) { //change something } : set up the change in responsive breakpoints webpage

 > Combine selectors:
  >> .selector1, .selector2 {}: apply to all selectors appear
  >> #id .class {}: select class that has parents as #id
  >> .class1.class2 {} :select element that has 2 classes

- Other assorted useful properties:
 > Opacity: 0 - 1: the transparant of the "entire element"
 > Transition: property name | duration | timing function | dalay
  >> transition: background-color 3s 1s; -- 3s needed take to change background color after 1s delay
  >> timing function: linear | ease-in | ease-out | ease | ease-in-out
 > transform: rotate | scale | translate(moving) | skew
  >> transform-orgin: center | top-left | bottom-right
 > background:
  >> background-image: url("/.././...")
  >> background-size: contain | conver | auto
  >> background-position: top | left | center ...
  >> background-repeat: no-repeat
  >> background: image| size | repeat | ...
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
  
  **5. JavaScript**
    <details><summary>Collapse</summary><p>
  <details><summary>Javascript</summary><p>
 
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
   
 >> console.log | console.error | console.warning
 >> Truthy and False: everything that is not (false | 0 | "" | null | undefine | NaN) are true.
 >> parseInt: parse a string argument and return an integer
 >> Object.keys({objectName}): return the keys of the object in an array
 >> Object.values({objectName}): return the values of the object in an array
 >> Object.entries({objectName}): return the nested array of key-value pairs
 
 
   
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
  >>> shift and unshift: remove / add from start
   >>> concat: merge array
   >>> includes: look for a value
   >>> indexOf: just like string.indexOf
   >>> join: create a string from an array
   >>> reverse: reverse an array
   >>> slice: copy a portion from an array. Can be used with "negative index"
   >>> splice (start[, deleteCount[, item1 [, item2 [, item3]]]]): remove / replace element
   >>> sort: sort an array
 
 >> While loops: while (something is true) {//Do something}
  >> while (i < 2) {
     console.log(i)
     i++ ; 
     }
 >> For loops: for (i = 0; i < 2; i++) { // Do something}
  >> i = 0 : start
  >> i < 2: end
  >> i++: change step
   
 > For ... OF / IN:
   >> for (variable of iterable) {statement}
   >> example: 
   >>> const subreddits =  [sub1, sub2, sub3, sub4];
   >>> for (let sub of subredits) {console.log(sub)};
   >>> for (let char of "Hello World!") {console.log(char};
   >>> for (let person in testScore) {console.log(`${person} scored ${testScore[person]}`)}
   
 >> Function:
  - Returning  functions:
   >>> function makeBetweenFunc(min, max) {
       return function () {
         return num >= min && num <= max;
       }}
   >>> const isChild = makeBetweenFunc(0,18);
   >>> isChild(7) //true
   >>> isChidl(40) // false
  - Higher Order Function:
   >>> function callTwice(func) {
       func();
       func();
       }
  - Defining Methods:
   >>> 
 ```
 </p></details>
 
 <details><summary>DOM</summary><p>
 
 ```python
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
 <details><summary>JQuery</summary><p>
 
 ```python
 
 > $ = document.querySelector / document.querySelectorAll
   >> $("h1").css("color", "red"): change the css color to red of h1
 > $("h1").addClass("big-title margin-50"): add class ".big-title" and ".margin-50" to "h1".
   >> .addClass: add class to element ("big-title");
   >> .removeClass: remove class from element ("big-title");
   >> .hasClass("big-title"): true
   >> .text("Bye"): change the text inside the HTML to "Bye"
   >> .html("<em>Don't Click Me</em>");
   >> $("a").attr("href", "https://www.google.com"); change the attribute

>> addEventListener:
   >>> $("h1").click(functionc () { //Do something});
   >>> $("button").click(function () {
       $("h1").css("color", "red");
   })
   >>> $("input").keydown(function (event) { console.log(event.key); })
   >>> $("h1").on("mouseover", function () {$("h1").css("color", "red")}) : apply to all methods
   >>> "on" method: https://developer.mozilla.org/en-US/docs/Web/Events
   
   >>> adding and removing element: 
      - before / after: $("h1").before("<button>New button</button>"): add element before / after the h1
      - prepend / append: $("h1").prepend("<button>New button</button>"): add element before / after the content of h1
      - $(button).remove(): remove all the button elements
      
 >> Animations: https://www.w3schools.com/jquery/jquery_ref_effects.asp
   >>> hide() / show() / toggle(): $("h1").hide(): affect the flow of the HTML
   >>> fadeOut() / fadeIn() / fadeToggle(): it fade the elementb before hide it
   >>> slideUp() / slideDown() / slideToggle(): slide the item before hide it
   >>> Animate: $("h1").animate({opacity: 0.5}): change the custom animation
      
 ```
 </p></details>
 </p></details>
</p></details>

---

<details><summary>BACK-END</summary><p>
1. NodeJs: install: npm init

```javascript
 - node myFile.js //Run the node file 
 - process.cwd() //print the current directory
 - process.argv // return an array containing the command line arguments passed when the NOde.js process was launched
 - npm link "packageName" : link the global package to the current folder
 - package.json: record of package
  >> npm init: creating package.json file
  >> npm install : it look for the package.json and install all the dependencies
  >> 
 
 ```
2. Expressjs: http://expressjs.com/en/5x/api.html#app.set
<details><p>

```javascript
- Install: 
>> npm install express
>> const express = require("express");
>> const app = express();
>> const port = 3000;

- Handling Request and Response:
>> app.set(name, value); //assign the setting name to value
  - When using 'view engine': we must create a folder called 'views'

// Change the path directory:
 >> const path = require('path');
 >> app.set('views', path.join(__dirname, '/views') // join the path in the parentheses
 
- Get request: used to retrieve information, data is sent via query string, limited amount of data can be sent 
>> app.get("/", (req, res) => res.sendFile(__dirname + "index.html")); 
>> app.get("/", (req, res) => res.send("Contact me at: nickpham163@gmail.com")); //we can use res.write with combination of res.send
>> app.get('/', (req, res) => res.render('home'); //render the HTML file home 

- Post request: used to post data to the server, used to write/create/update. Can send any sort of data (JSON) via request body, not a query string
>> app.use(express.urlencoded({extended: true}));
>> app.post("/", (req, res) => {...}); route the HTTP POST request to the specify path with the specify callback function
 >>> req.body.idName : idName must match with the name of the input
 
>> app.use(express.static("{folderName}"); //link the css sources and imgages to the html
>> app.use(() => console.log("We got a new request!!!!")) //anytime we hit refresh, this code run

-  Serve static assest: express.static(root, [optional]);
>> const path = require('path')
>> app.use(express.static(path.join(__dirname, "/public")));

>> app.listen(port, () => console.log("Server is running on port 3000"));


 
>> Express Path Parameter:
  >>> "/:something" :checking for pattern like an variable
 
>> Query String:
  app.get("/search", (req, res) => {
  const { q } = req.query;
  if (!q) {
    res.send("Nothing found")
  }
  res.send(`<h1>Search result for: ${q}</h1>`)
  })
  
- Templating EJS language: https://ejs.co/
 - in Index.js: app.get('/', (req, res) => {
                const num = Math.floor(Math.random())
                res.render('random', {num})
                });
 - in random.ejs: <h1>Your random number is <%= num %></h1>
 
- CONDITION in EJS:
 >> <h3><%= rand % 2 === 0 ? "Even" : "Odd" %></h3>
 
- LOOP in EJS:
 >> <ul> 
    <% for (let cat of cats) { %>
 <li> <%= cat %> </li>
   <% } %>
    </ul>
    
- Includes:
 <%- include ('partials/navbar') %>

- Nodemon: automatically restarting the node application when file changes in directory are detected
>> install: npm install -g nodemon
>> usage: nodemon [your node app]

- body-parser: extracts the entire body portion of an incoming request stream and exposes it req.body
 >> install: npm install body-parser
 >> const bodyParser = require("body-parser");
 >> app.use(bodyParser.urlencode({extended: true}));

- REST - representation state transfer:


 ```
</p></details>
 
3. APIs: Application Programming Interfaces
 <details>
  
  ```python
  
 - Definition: an application programming interface (API) is a set of commands, functions, protocols, and objects that programmers can use to create software or interact with an external system.
 - JSON: Javascript Object Notation:
   >> JSON.parse(data): turn data into json viewer awesome
   >> JSON.stringify(data): turn data into flat
  > HTTPS:
   >> const https = require("https")
   >> app.post("/", (req, res) => {
       let cityName = req.body.cityName;
       let apiKey = {key}
       https.get("http:// .... ?q=${cityName}&appid=${apiKey}", (resonse) => {
         response.on("data", (data) => {
         const weatherData = JSON.parse(data); //convert data to JSON
         let temp = weatherData.main.temp;
         let icon = weatherData.weather[0].icon;
         let iconurl = `http://openweathermap.org/img/wn/${icon}@2x.png`
         let iconImage = `<img src = ${iconurl}>`
         res.write(`The temp is ${temp} degrees Celcius.`);
         res.write(iconImage);
         res.send();
         })
       })
       })
  
 ```
</details>

4. React - Portfolio:
<details>

``` ruby
- JSON packages:
 >> @sanity/client
 >> @sanity/image-url
 >> framer-motion
 >> node-sass
 >> react-icons
 
- Steps:
 >> Create folders named: aboutm header, footer, skills, testimonials, works.
 >> Create jsx files and scss files inside the container as schemas
 >> Create other folders called: assets, components, constants
 >> Inside components, create Navbar folder and 2 files inside Navbar.jsx and Navbar.scss
 
- Connect to Sanity to Fetch Data:
 >> create a client.js file in 'back-end folder' (look the file in porfolio project)
  >>> terminal: sanity manage - to get all information for client file
 >> create a .env file in 'front-end folder' to secure the "projectId" and "token"
  >>> terminal: sanity start - compile and fetch data at defined localhost
 
 
 
 
 
 
</details>
