##  Less obvious strings

**Nope:**

```html
<img alt="A lovely sunset" src="sunset.jpg">
```


```js
var text = 'A thing I want to say';

throw new Error('The request failed')
```

**Yep:**

```html
<img alt="{ __('lovelySunset') }" src="sunset.jpg">
```


```js
var text = __('thingToSay');

throw new Error( __('errors.requestFailed') )
```



note:

When you start thinking this way, you realize you're using strings everywhere. Attributes, variables, messages… they're everywhere. And you can't just write one anymore.

This is why I said it's better to start early.
