# ⇪ Caps Drag
Break free from the shackles of dragging stuff on your mac. Maybe this isn't a problem for anyone else (?), but using the first gen Apple track pad I have at home these past few weeks of quarantine has been _killing_ my forearm. Seriously. Fearing RSI, carpal tunnel, I put my head down and found a better way.

## Problem to solve
- break free from the tyranny of longpress while dragging
- leverage macOS’s accessibility settings for alternative control methords, while circumventing their keystroke limitations
- repurpose unused ⇪ `caps lock` key, toggling drag by _ever so slightly_ lifting a pinky finger on your left hand

## Quick start
Setup requires mapping an accessibility switch to drag, mapping that key to caps lock, and moving a script to perform the script each time your Mac boots up.
1. From System Preferences > Accessibility > Pointer Control > Alternative Control Methods check ✅ "Enable aternative pointer actions" and configure **Options…**
1. hit plus + to add a new Physical Switch
1. hit F13 on external keyboard
1. Place **com.user.hidutilScript.plist** in `{user}/Library/LaunchAgents/com.user.hidutilScript.plist`
1. Move **hidutilScript.zsh** to `{user}/Library/logs/hidutilScript.zsh`