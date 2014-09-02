title: Javascript Basics
author:
  name: Justin Donato
  twitter: justindo
  url: http://justindonato.com
controls: false
theme: matmuchrapna/cleaver-ribbon

--

# Javascript in the Browser

-- 

- HTML: Structure (What it is)
- CSS: How it looks (and moves)
- Javascript: What it does.

-- 

# Document Object Model (DOM)

- The computer's internal representation of your markup.
- A "Tree-like" structure
- Each element is a "Dom Node"
- Different than "View Source"
- Javascript can read and change it.

-- 

# window

- Javascript's environment in the browser
- Provides access to Javascript Built-ins...
- There's tons of stuff on window. Go explore.

```javascript
// Try this: go to: https://www.google.com/?q=cats
var loc = window.location.toString();
window.location = loc.replace('google', 'bing')
```

-- 

# window

- Also provides access to the DOM through (window.document)

```javascript
window.document.body.style.backgroundColor = 'red';
```

-- 
# You can dynamically change nearly any part of the DOM.

To do so, you need a reference to a DOM Node.

```javascript
var myBox = document.getElementById('box');
var myBoxes = document.getElementsByTagName('div');
var myOrangeBoxes = document.querySelectorAll('.orange');
```

-- 

Once you have a dom node, you can...

```javascript

// Add a class using classList

var myBox = document.getElementById('box');

myBox.classList.add('orange');
myBox.classList.remove('bold');

```

-- 

Change styles directly

```javascript

var myBoxes = document.getElementsByTagName('div');
myBoxes[0].style.backgroundColor = 'red';

// Notice I use array access brackets to get the first element.
// You can't do myBoxes.style because my box is not a dom node, its a list of them.
```
-- 

You can remove an element.

```javascript
var myBoxes = document.getElementsByTagName('div');
var firstBox = myBoxes[0];
firstBox.remove();
```
-- 

You can create a new element

```javascript

var newDiv = document.createElement('div');
var text = document.createTextNode('Dynamically added text');
newDiv.appendChild(text);
document.body.appendChild(newDiv);
```
-- 

You can create a new element

```javascript

var newDiv = document.createElement('div');
var text = document.createTextNode('Dynamically added text');
newDiv.appendChild(text);
document.body.appendChild(newDiv);
```
