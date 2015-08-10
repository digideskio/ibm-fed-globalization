##  Multi-part strings

**Nope**:

```js
var greeting = 'Hello ' + user.name + '! You are '
  + user.age + ' years old'
```

**Yep:**

Resources:

```json
"greeting": "Hello __name__! You are __age__ years old"
```

```json
"greeting": "¡Hola __name__! Tiene __age__ años"
```


Later…

```js
var greeting = __('greeting', user)
```

note:

You can totally forget about building messages one tiny piece at a time, right? What if subject/verb order is different? What if there are differences in punctuation?

You can see in the second example a little bit of that with Spanish. The library I use lets you pass in an object and replace variables that way.

Personally, dealing with strings in this manner is a lot more pleasant than piecing them together with "+" sign.
