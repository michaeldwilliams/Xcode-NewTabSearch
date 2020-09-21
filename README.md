# Xcode New Tab Search

Applescript that opens the Quick Open search bar when you open a new tab.

### Why?
Let me answer this question with another question.
Why would I want to open a tab to the exact same file I was just in?

### How to Install
1. In a empty text file add the following and save it as a shell script:

```
#!/bin/sh

osascript {Location of your scpt file here}/Xcode-NewTabSearch.scpt
```

2. Make your script executable with `chmod u+x YourFileName.sh`
3. In Xcode, change the key binding for New Tab to something else (It's set to `shift+command+control+option+T` in the script file so you can set it to that if nothing else shares that same key binding or you need to change the script file.)
4. In Xcode, create a new Behavior (Preferences > Behaviors > +) and tick the run option selecting your shell script
5. Add a keybinding to the Behavior (I used `command+T` as the original intent was to replace the generic command for opening a new tab)
6. Xcode will prompt you to add the correct permissions in the system but after you do that, it should work.

Feel free to change the Applescript file to fit your needs.


Enjoy!
