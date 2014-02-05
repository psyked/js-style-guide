### Organise your source code
- Group your variable declarations together, and add them to the top of the function they're scoped into.
- Use named functions instead of anonymous functions (you'll thank me at debug time)

#### Best Practice
Don't nest your function declarations - doing so means that the nested functions are evaluated when the parent function
is executed, which prevents a lot of browser pre-optimisation and can get confusing to track the scope of variables used
in the function itself. Abstract those functions, or change their scope and be more explicit about the parameters passed
into that function.