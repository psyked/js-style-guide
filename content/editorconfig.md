### Sort out your auto-formatting.

Configure your IDE to have it follow these few simple rules for code formatting.

- Use **whitespace to improve the readability of your code** (ie, don't auto-condense blank lines)
- Keep your opening braces (`{`) **on the same line**
- Indent code with **4 spaces** (don't use tabs)
- Use **single quotes** in strings
- Use a single space after colons (`:`), around operators, keywords and parenthesis (`{`/`}`), but not within them.
- **Remove trailing whitespace** from lines of code
- Always use semicolons (`;`) at the end of lines (and don’t rely on implicit insertion.)

You may also wish to have your IDE display hidden characters (newlines, spaces, tabs), which will make these errors
easier to spot. And remember, too much whitespace throughout your code can make it just as hard to read as too little.

Ideally, your formatted code should look something like this:

    function foo(x, y, z) {
        bar(1, b);
        var i = 0;
        var x = {0: "zero", 1: "one"};

        var foo = function foo() {
            // stuff
        };

        if (!i > 10) {
            for (var j = 0; j < 10; j++) {
                switch (j) {
                    case 0:
                        value = "zero";
                        break;
                    case 1:
                        value = "one";
                        break;
                }
                var c = j > 5 ? "GT 5" : "LE 5";
            }
        } else {
            var j = 0;
            try {
                while (j < 10) {
                    if (i == j || j > 5) {
                        a[j] = i + j * 12;
                    }
                    i = (j << 2) & 4;
                    j++;
                }
                do {
                    j--;
                } while (j > 0)
            } catch (e) {
                alert("Failure: " + e.message);
            } finally {
                reset(a, i);
            }
        }
    }

> If in doubt, _Consistency always wins._

#### Best Practice
Use an [EditorConfig](http://editorconfig.org/) file to set this up for you.
Create an `.editorconfig` file in the root of your project, and then set up your IDE to use
those settings when auto-formatting your code.

    //todo: Add Sample file

<div class='panel'>
{{#markdown}}
**Useful resources:**
- [About EditorConfig](http://editorconfig.org/)
- [Configuring WebStorm to use EditorConfig](https://github.com/editorconfig/editorconfig-jetbrains#readme)
{{/markdown}}
</div>