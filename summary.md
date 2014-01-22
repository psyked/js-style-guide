---
title: The “Too long; didn’t read” Style Guide
---
<div class='row'>
<div class='large-12 columns'>
{{#markdown}}
1. Configure your IDE with Files & Plugins
------------------------------------------
</div>
<div class='large-6 columns'>
### Use a [JSHint](http://www.jshint.com/about/) file.
Create a `.jshintrc` file with the following content in the root of your project, and configure your IDE to continually
validate your source code against those settings during development.

    {
      'camelcase' : true,
      'indent': 4,
      'undef': true,
      'quotmark': 'single',
      'maxlen': 120,
      'trailing': true,
      'curly': true,
      'es3': true,
      'strict': true,
      'eqeqeq': true,
      'browser': true,
      'jquery': true
    }

- [Configuring WebStorm to use JSHint](http://www.jetbrains.com/webstorm/webhelp/using-javascript-code-quality-tools.html)

</div>
<div class='large-6 columns'>
### Use an [EditorConfig](http://editorconfig.org/) file.
Create an `.editorconfig` file with the following content in the root of your project, and then set up your IDE to use
those settings for auto-formatting your code.

<pre><code class='no-highlight'># EditorConfig is awesome: http://EditorConfig.org

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
</code></pre>

- [Configuring WebStorm to use EditorConfig](https://github.com/editorconfig/editorconfig-jetbrains#readme)
</div>
</div>
<div class='row'>
<div class='large-12 columns'>
2. Use the proper formatting conventions.
-----------------------------------------
Use descriptive function and variable names, in the format:

- `functionNamesLikeThis`
- `variableNamesLikeThis`
- `ClassNamesLikeThis`
- `EnumNamesLikeThis`
- `methodNamesLikeThis`
- `CONSTANT_VALUES_LIKE_THIS`
- `foo.namespaceNamesLikeThis.bar`
- `filenameslikethis.js`

Use a consistent vocabulary like is, has, set and get:

- `function isReady()`
- `function hasValue()`
- `function setName()`
- `function getName()`

Use whitespace as outlined by the [Idiomatic JavaScript Style Guide](https://github.com/rwaldron/idiomatic.js/#spacing)

Braces go on the same line, not a new line.
{{/markdown}}
</div>
</div>
