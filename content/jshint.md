### Add a [JSHint](http://www.jshint.com/about/) file.
Create a `.jshintrc` file with the following content (or [download it here]()), add it to the root of your project and validate your source code
against it during development.

    {
      'camelcase' : true, // naming conventions
      'indent': 4, // 4 space indent
      'undef': true,
      'quotmark': 'single', // use single quotes
      'maxlen': 120,
      'trailing': true,
      'curly': true, // always use curly braces
      'es3': true, // for backwards compatible code
      'strict': true, // for predictable code
      'eqeqeq': true, // === instead of ==
      'browser': true, // console.log, etc.
      'jquery': true // adds $ as a valid function
    }

#### Best Practice
Set up your IDE to continuously validate against the JSHint rules as you work, and have any Continuous Integration setup
 do the same.

<div class='panel'>
{{#markdown}}
**Useful resources:**
- [About JSHint](http://www.jshint.com/about/)
- [Configuring WebStorm to use JSHint](http://www.jetbrains.com/webstorm/webhelp/using-javascript-code-quality-tools.html)
{{/markdown}}
</div>