##  Don&#39;t repeat languages

**Better!**

```bash
/de
/en
/es
/fr
/it
/ja
/ko
/pt
/zh
/zh-TW
```

**Express configuration**

```js
app.use('/locales/zh-Hant', express.static('locales/zh-TW'));
```

note:

One trick is to only get specific if you absolutely have to. For example, most translation libraries assume if you say "Portuguese" but don't specify a country, they assume you meant Brazil. Same with English and the United States. So you can work with only the language code instead of languages and countries.

If you can't get away with that, have your server serve a single directory of files to multiple requests so you don't have to copy the files all over the place. In that second snippet, the server will use the same files for a request for zh-Hant as it would for the identical zh-TW. One line of code, so much sanity saved forever.
