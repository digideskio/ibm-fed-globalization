#  Use the machines

note:

Definitely look into automating as much as you possibly can.

For example, our app has a task that runs that scans all of our HTML and JavaScript files, sees every time we run the i18next functions, collects the keys, and automatically updates the resources JSON files.

So every time we save a file, the JSON has already been updated. If we stop using a string, this task has already removed it. I estimate that this little task has saved me approximately a billion years. At least that's what it feels like.
