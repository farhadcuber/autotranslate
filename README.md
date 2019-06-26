Select a word and use a shortcut key to notify the meaning in Farsi.
Using [translate-shell](https://github.com/soimort/translate-shell).

# Dependencies
1. xbindkeys
2. xsel
3. curl
4. notify-send (for install it on ubuntu $ apt install notify-osd)
5. gawk

# Installation
After installing xbindkeys create a .xbindkeysrc file<br />
    xbindkeys --defaults > ~/.xbindkeysrc

add append these lines to ~/.xbindkeysrc<br />
    _"bash pathTofiles/seltr"_<br />
    _m:0x15 + c:52_<br />
    _Control+Shift+Mod2 + z_<br />

for Example in my case:<br />
    "~/autotranslate/seltr"<br />
    m:0x15 + c:52<br />
    Control+Shift+Mod2+z<br />

to apply changes enter following commands:
    `killall -s1 xbindkeys`
    `xbindkeys -f ~/.xbindkeysrc`
  

# Usage:
1. Select the word.
2. Use shortcut Ctrl + Shift + z.
