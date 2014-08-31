title: Javascript Basics
author:
  name: Justin Donato
  twitter: justindo
  url: http://justindonato.com
output: basics.html
controls: false
theme: sudodoki/reveal-cleaver-theme
--

# Javascript Basics

--

All examples in class will assume you're using Chrome unless otherwise specified.

--

# Developer Tools

(right click and choose 'inspect element')

--

# HTTP and the Browser

--

Running javascript.

```javascript
<p>Hello World</p>
<script>
    console.log('Hello World');
</script>
```

or

```javascript
<p>Hello World</p>
<script src="my-script.js"></script>
```
--
# Comments

```javascript
// Inline Comment

/* Multiline
   comment */
```

--

# Keywords vs. Built-Ins vs. User Names

--

# Variables

Think of them as names that point to data

```javascript

// Create a variable with a name
var myVariable; // Notice the semi-colon.

// Create a variable and initialize it with a value
var myOtherVariable = 1;

// Use a variable

console.log(myOtherVariable);

// Change a variable's value
myOtherVariable = 2;
```

--

# Types of Values

Numbers, Strings, Booleans


```javascript
"A String"
100
1.2
true
```

--

# Variables can hold any Type


```javascript
var name = "Dingbat";
name = 750;
name = true;

```

--

# Operators

Perform operations on data. Meaning is defined by the types they are operating on. 


```javascript

// What do these do?

5 + 4;

"Humpback " + "Whale";

5 + "Whale";

"Whale" - 5;

```

--

# Boolean Operators

Allow you to do complicated logic

```javascript

var isStudent = true;
var isEmployee = true;

var isSortOfTired = isStudent || isEmployee;
var isReallyTired = isStudent && isEmployee;

var hasGraduated = !isStudent;


```

--

# Undefined and Null

Special types. They mean: there is no data.

```javascript
var myVar; // undefined
var myOtherVar = undefined; // undefined is also a keyword.
var nothing = null;
```

You can think of null as an explicit way of saying, I want this variable to have no value

--

# Complex Data Types: Arrays 

lists of things. Use '[' and ']' to make them.


```javascript
var plants = ['cactus', 'aloe', 'basil', 'olive tree'];
var weirdList = ['rocking chair', 14, true, 5 - 2];

// access items using numeric indices:

plants[0]; // 'cactus'
plants[1000]; // undefined
```

--

# Complex Data Types: Objects

Collections of named data. 


```javascript
var course = {
    title: 'javascript',
    day: 'Monday',
    students: ['Jane', 'Bob', 'Jung']
};

// access data using names

course['title']; // 'javascript'
course['students'] // ['Jane', 'Bob', 'Jung]
course['students'][0] // 'Jane'

// or you can use 'dot' syntax
course.title // 'Monday'

```
--

Objects can be nested


```javascript
var courseLoad = {

    'javascript' : {
        title: 'javascript',
        day: 'Monday',
        students: ['Jane', 'Bob', 'Jung']
    },

    'printmaking' : {
        title: 'printmaking 101',
        day: 'Tuesday',
        students: ['Jane', 'Tina', 'Emmet']
    }

};


```
--

```javascript

var student = {};

student.name = 'Jim';
student.average = 2.7;
student.year = 2017;

```
--

# Methods and Properties

Javascript types have various ways of getting data about the data they store or manipulating that data.

```javascript

var sentence = "The Quick Brown Fox Jumped Over The Lazy Dog";
console.log(sentence.length);

sentence = sentence.replace("Brown", "Pink");
console.log(sentence);

```
