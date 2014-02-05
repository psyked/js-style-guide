### Follow the camelCase/CamelCase naming conventions
In addition to using descriptive names, we convey an objects' type through the **camelCase** conventions. JavaScript
isn't case-sensitive, but it promotes better clarity in our source code.

##### Functions & variable declarations
Use lower camelCase. Compound words, where each word begins with a capital letter, with the exception of the first letter.

    var myReallyLongVariableName;

    function myReallyLongComplicatedFunctionName() {
        // stuff
    }

##### Class declarations
Use upper CamelCase. Compound words, where each word begins with a capital letter, including the first letter.

    var ClassName = function ClassName() {
        // stuff
    };

##### Constants
Are signified with ALLCAPS and separate words signified by underscores.

    var MY_CONSTANT = 42;

##### Nested properties
Are best accessed via dot-notation, rather than `eval` blocks. (Eval is Evil)

##### Filenames
Use all-lowercase file names, and preferably separate words with dots rather than hyphenating filenames.

`my.complicated.filename.js` rather than `my-complicated-filename.js`