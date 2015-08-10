#  Headers are your friend

note:

The only reliable way I've found to detect language is server-side, using `Accept-Language` headers. Despite all that weirdness with the DOM, browsers always get this right.

Only detect languages using those headers, and only do so server-side.
