---
title: JavaScript Style Guide
---
<div class='row'>
<div class='large-4 columns'>
{{#markdown}}
## ** tl;dr **
Background reading can get a little boring, so you can skip past that and onto the good stuff by reading our summary.

<a href='summary.html' class='button'>Open the Summary now.</a>
{{/markdown}}
</div>
<div class='large-8 columns'>
{{#markdown}}
    if (isNewProject) {
        shouldUseThisStyleGuide = true;
        shouldMinifyJavaScript = true;
    }

    if (shouldUseThisStyleGuide) {
        applyIDEFormattingPreferences();
        integrateJSHintFile();
    }

    if (shouldMinifyJavaScript) {
        buildTool = BuildTools.GRUNT;
        minificationLibrary = 'uglifyjs';
        makeCompatibleWithOldIE = true;
    }
{{/markdown}}
</div>
</div>

<div class='row'>
<div class='large-6 columns'>
{{#markdown}}
#### Background reading:
Our JavaScript Style Guidelines are drawn from a combination of many sources, but primarily from the following sources:
- [JavaScript, the winning style](https://github.com/Seravo/js-winning-style)
- [Principles of Writing Consistent, Idiomatic JavaScript](https://github.com/rwaldron/idiomatic.js/)
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- [Google JavaScript Style Guide](http://google-styleguide.googlecode.com/svn/trunk/javascriptguide.xml)
- [Render-blocking javascripts](http://www.feedthebot.com/pagespeed/render-blocking.html)
{{/markdown}}
</div>

<div class='large-6 columns'>
{{#markdown}}
{{/markdown}}
</div>
</div>