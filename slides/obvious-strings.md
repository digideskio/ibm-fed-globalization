##  Obvious strings

**Nope:**

`<a href="#">Back to Dashboard</a>`

**Yep:**

`<a href="#">{ __('backToDashboard') }</a>`

note:

Sometimes, strings are obvious. Text in an element that gets displayed. Easy.

Every place that you would have text, you will instead have a function that looks for a translated version of that text. Every single time.

I'm showing these examples using the Dust template language, and I've created a shortcut "double underscore" function to look up text by key.
