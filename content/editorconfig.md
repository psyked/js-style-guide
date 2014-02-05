### Sort out your formatting.
**Standard Practice:**
Follow these simple rules for code formatting:

- Keep your opening curly braces (`{`) **on the same line**
- Indent code with **4 spaces** (don't use tabs)
- Use **single quotes** for String declarations
- Use a single space after colons (`:`), around evaluations and before `{`, like this:


    if(var i = 0, l = 10; i < l; i++) {
        // stuff
    }

- Use whitespace to improve the readability of your code
- Move your `var` statements to the top of their scope (function)
- Use named functions instead of anonymous functions (you'll thank me at debug time)

> If in doubt;
> Consistency always wins.

**Best Practice:**
Use an [EditorConfig](http://editorconfig.org/) file to set this up for you.
Create an `.editorconfig` file in the root of your project, and then set up your IDE to use
those settings when auto-formatting your code.

    //todo: Add Sample file

<!-- <pre><code class='no-highlight'># EditorConfig is awesome: http://EditorConfig.org

# top-most EditorConfig file
root = true

# Unix-style newlines with a newline ending every file
[*]
end_of_line = lf
insert_final_newline = true

# 4 space indentation
[*.py]
indent_style = space
indent_size = 4

# Tab indentation (no size specified)
[*.js]
indent_style = tab

# Indentation override for all JS under lib directory
[lib/**.js]
indent_style = space
indent_size = 2

# Matches the exact files package.json and .travis.yml
[{package.json,.travis.yml}]
indent_style = space
indent_size = 2
</code></pre> -->

<div class='panel'>
{{#markdown}}
**Useful resources:**
- [About EditorConfig](http://editorconfig.org/)
- [Configuring WebStorm to use EditorConfig](https://github.com/editorconfig/editorconfig-jetbrains#readme)
{{/markdown}}
</div>