#### Globals
Don’t use globals. “Global name conflicts are difficult to debug, and can cause intractable problems when two projects try to integrate. In order to make it possible to share common JavaScript code, we’ve adopted conventions to prevent collisions.”

#### Be Strict
In any kind of JavaScript file it is also good to add the declaration:

    'use strict';

This will affect both JSHint and your JavaScript engine, which will become less compliant but should execute your JavaScript faster through internal use of a more optimised engine.

#### Check for absolute equality
Use `===` and `!==` instead of `==` and `!=`. See the post [Truth, Equality and Javascript](http://javascriptweblog.wordpress.com/2011/02/07/truth-equality-and-javascript/) for more information on exactly why you should do this.

#### Function parameters - required & optional values
The following words of wisdom should help you write a better structured code in Javascript:

- Keep the number of parameters required by a method to a minimum.
- Required parameters go first.
- Optional parameters go last.
- If there’s more than a single optional parameter, supply the values as an object with the optional values as parameters of that object.

Thus:

    function myReallyCoolMethod(required, options);

Is better than:

    function myReallyCoolMethod(required, required, required, optional, maybeoptional, required);

We can easily guess how that sort of code emerges - but honestly, refactor your code instead of adding new parameters to your functions.

#### One function, one effect. One Class, one responsibility.
As you develop, your classes and methods should only have one responsibility. Avoid cramming too much functionality into a single class or method, and be wary of creating functions that have side effects without making them explicit.