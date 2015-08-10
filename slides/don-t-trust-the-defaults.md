##  Don&#39;t trust the defaults

**i18next defaults options:**

```json
{
  useCookie: true,
  fallbackLng: "dev",
  fallbackOnNull: false
}
```

note:

These are some of the default options for i18next. They are troublesome.

By default, i18next tracks languages with a cookie. As we'll discuss in a moment, that's a dumb idea.

It also assumes that there will be a language to fallback to named "dev", which is a not a language I've ever heard of. Change that to English.

It also doesn't try to use a fallback by default. Maybe you like that.
