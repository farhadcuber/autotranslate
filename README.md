Select a word and use a shortcut key to notify the meaning in Farsi.
Using [translate-shell](https://github.com/soimort/translate-shell).

# Dependencies
1. xbindkeys
2. xsel
3. curl
4. notify-send (for install it on ubuntu $ apt install notify-osd)
5. gawk

# Installation
After installing xbindkeys create a .xbindkeysrc file
`xbindkeys --defaults > ~/.xbindkeysrc`

append these lines to ~/.xbindkeysrc
```
"bash pathTofiles/seltr"
m:0x15 + c:52
Control+Shift+Mod2+z
```

for example in my case:
```
"~/autotranslate/seltr"
m:0x15 + c:52
Control+Shift+Mod2+z
```

to apply changes enter following commands:
```
killall -s1 xbindkeys
xbindkeys -f ~/.xbindkeysrc
```
  

# Usage:
1. Select the word.
2. Use shortcut Ctrl + Shift + z.
