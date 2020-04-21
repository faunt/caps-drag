# ⇪ Caps Drag
Do you drag stuff? Do you drop it? Do you like using CAPS LOCK? Do you have long finger nails and gentle hands like me? 

If you answered yes and no to those questions, **⇪ Caps Drag** might be for you.

It's for anyone who _ya, now that you mention it, dragging stuff **does feels like being handcuffed** to my mac_. A productivity and ergonomics hack for anyone with accessibility needs to _barely lift a pinky finger_ in their daily work.

With **⇪ Caps Drag**, you can drag and scrub and resize and draw boxes by literally _barely_ lifting your pinky finger. Your left pinky finger. And putting it on the caps lock key. Then effortlessly waving a single finger across your trackpad to draw before dropping with that gentle pinky again.

No more claw hands contorting, clenching, killing. Relax. Lift those pinkies. Do more better and faster. Everything is fine now.

## Problem to solve
- break free from the tyranny of longpress while dragging
- leverage macOS’s accessibility settings for alternative control methods, while circumventing their keystroke limitations
- repurpose unused ⇪ `caps lock` key, toggling drag by _ever so slightly_ lifting a pinky finger on your left hand

## Quick start
Setup requires mapping an accessibility switch to drag, mapping that key to caps lock, and moving a script to perform the script each time your Mac boots up.
1. From System Preferences > Accessibility > Pointer Control > Alternative Control Methods check ✅ "Enable aternative pointer actions" and configure **Options…**
1. hit plus + to add a new Physical Switch
1. hit F13 on external keyboard
1. Place **com.user.hidutilScript.plist** in `{user}/Library/LaunchAgents/com.user.hidutilScript.plist`. Update `{user}` to your username by opening the `.plist` in a code editor
1. Move **hidutilScript.zsh** to `{user}/Library/logs/hidutilScript.zsh` or wherever so long as you update `.plist` the step above

## To do
- [ ] validate whether this deserves even a minute more time. Does anyone benefit from this?
- [ ] does Magic Trackpad gen 2 solve this? If hard press on gen 1 goes away, is there still a need?
- [ ] touchbar laptops: need to learn more about touchbar button mappings; Apple’s technical note [TN2450](https://developer.apple.com/library/archive/technotes/tn2450/_index.html) pertains to USB keyboard spec, so only seems to work for connected keyboards
- [ ] bundle as a one-time download and install utility
- [ ] icon, brand, marketing ?!

## FAQ
> But what if I still want to use caps lock?

Don’t. Just stop.




