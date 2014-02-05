### Use Descriptive Names for your objects

Make your code more readable by using full, descriptive names for your functions, variables and
objects. Don't try to save bytes by using short, terse variable names (with the exception of `i` in a loop).

#### Best Practice
Don't try to express concepts such as the object type, its scope or anything else through a pseudo
convention. <br>That means no `oObject` or `customersArray`, `_private` or `_this` variable names.

##### Bad code:

    // Example of code with poor names

    function q(s) {
      return document.querySelectorAll(s);
    }
    var i,a=[],els=q("#foo");
    for(i=0;i<els.length;i++){a.push(els[i]);}

##### Good code:

    // Example of code with improved names

    function query( selector ) {
      return document.querySelectorAll( selector );
    }

    var idx = 0,
      elements = [],
      matches = query("#foo"),
      length = matches.length;

    for ( ; idx < length; idx++ ) {
      elements.push( matches[ idx ] );
    }

Also, pay attention to plural and non-plural names when coding:

    var dog; // is a string

    var dogs; // is an array of dog strings

### Use a consistent vocabulary
Stick to an obvious set of keywords such as `is`, `has`, `set` and `get` for your simple accessor functions:

    function isReady() {};
    function hasValue() {};
    function setName() {};
    function getName() {};
