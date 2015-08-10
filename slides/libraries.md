## Outside libraries

![Our library that creates modal dialogs had hard-coded buttons](resources/modal-library.png)

note:

Which leads us to another consideration: if you're using someone else's code, do they let you customize the strings?

What I'm showing here is our UI using one of the many libraries for creating modal dialogs.

Do you know why we chose this particular one? Because it let us override the default "Cancel" and "OK" buttons with our own translated text.

If you use libraries that use text _anywhere_ and don't let you override it, well, you really can't use that library.
