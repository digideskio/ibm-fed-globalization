## Client-side language detection

**Nope :(**

```js
navigator.language
```

**Nope :(**

```js
navigator.languages
```

**Nope :(**

```js
navigator.userLanguage
```

note:

Here's an incomplete list of issues around detecting language in the browser.

That first one, navigator.language, in Chrome is permanently the language in which you _downloaded_ Chrome. It doesn't change with your preferences. Also, not in IE.

That second one, `languageS`, Chrome will inject extra languages in there against your will. Also, not in IE.

that `userLanguage` one, that one is Internet Explorer, but it reflects your system preference, not the language preference in the browser. Cute. If anyone has a reliable way to detect the preferred language in the browser, I'd love to hear it.
