### Sort out your auto-formatting.
**Standard Practice:**

**Best Practice:**
Add an [EditorConfig](http://editorconfig.org/) file.
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