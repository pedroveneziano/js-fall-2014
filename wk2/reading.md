Reading
=======

Read all of [Chapter 1](http://eloquentjavascript.net/01_values.html) and up to and including the section called "Mutability" in [Chapter 4](http://eloquentjavascript.net/04_data.html) of Eloquent Javascript.

Exercise
=========

To complete these exercises, you'll make a html file with a script tag. Complete the tasks below, adding console.log statements so you can see the results of each task. Keep refreshing the page in your browser and checking your console as you work. Commit your work to your repository and push it to github.

- Make a variable that holds a number. 
- Make a variable that holds another number.
- Make a variable that holds a sentence.
- Make a variable that holds the result of adding the two number variables.
- Make a variable that holds the result of adding one of the number variables to the sentence variable.
- console.log the result of subtracting the variable that holds a number from the variable that holds the sentence.
- Make an array containing all the names of your classes this semester.
- Make an object that has your course names as keys and instructor names as their values. Here I'll do mine:

```javascript
var classes = {
    'javascript': 'Justin Donato'
};
```

- Below is a function called `print` that logs the values passed to it. Make a function called `swap` that takes two values and logs them in reverse. For example:

```javascript

    var print = function(first, second) {
        console.log(first, second);
    };
    
    print(4, 5);
    // logs 4, 5
    print(10, "Hello");
    // logs 10, "Hello"
    
    // Now you write swap so that:
    // swap(1 ,2);
    // logs 2, 1
```
