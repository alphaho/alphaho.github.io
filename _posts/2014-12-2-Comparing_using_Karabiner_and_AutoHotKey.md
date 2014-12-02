---
layout: post
title: Comparing using Karabiner on Mac to AutoHotKey on Windows
---

I've been using Karabiner \(formerly known as KeyRemap4MacBook) on Mac and AutoHotKey on Windows for sometime.

Both are popular key remapping tools in the correpondent platform.

Here's some difference I have found between them, some of them I think are because of the differences of the underlying operating system.

#### 1. Karabiner has better system-wide support while AutoHotKey doesn't.
In Mac, the remapping can also take effect in the login window. While in Windows, it can't.  
What's more, in Windows, when I am using the application that runs in "Administrator Mode", the remapping fails again.

Combined with the Truly Ergonormic Keyboard I use, it's a better experience in Mac than in Windows, as I don't need to worry my remapping doesn't work.

#### 2. AutoHotKey supports switching to a specific application or a group, while Karabiner doesn't.
Following [Xah Lee's suggestion](http://xahlee.info/kbd/set_single_key_to_switch_app.html), it's very handy to bind a key to an application. So you can maybe press F1 and switch to Emacs, press F2 and switch to the browser and so on. This has dramatically speeded up my daily workflow in Windows and helps a lot when I need to switch between different applications(Emacs, browser, IntelliJ, IM, mail client, Windows Explorer, etc.). I almost don't need to move my mouse to the task bar, look for the appliaction I want(What's worse, I may even forget which app I am looking for at this stage), click on it, move the mouse to the place I'm interested in. And so on.

You can also rotate the different windows if you keep pressing the same key. For example, if I have multiple instance of Emacs, I can keep pressing F1 \(the key I've bound to Emacs) and the different instance will show up.


But, on Mac, Karabiner doesn't support this feature out of the box. Maybe it can, throught calling an AppleScript. I may find it out later.  
However, the good side of using Mac is, the OS itself support rotating the different instance within the same application. \(You can find out or set this shortcut in "System Preferences.." -> "Keyboard" -> "Shortcuts" -> "Keyboard" -> "Move focus to next window") And the Cmd-Tab application switching switches the focus from application to application, rather than from window to window.  
This makes it easier when we don't have the same application specific key as with AutoHotKey.

#### 3. Karabiner supports device specific and layout specific bindings.
This makes it easier to switch between different keyboards and layouts. The remapping won't mess up.

For example, this has make my life easier when I switch between the Apple intenal keyboard and my Truly Ergonormic keyboard.  

As I would use Workman system layout with my internal keyboard while I would use U.S. stanard layout with my TECK. If I don't have two sets of settings for these two combinations, the remapping won't work at one of the keyboard as the underlying key codes are different. This makes one of my keyboards not so usable.
After setting it up, I now have the both keyboards works with the same remapping and I don't need to remind myself that "don't use this key combination as I have switched my keyboard". 

What's more, while I am setting the remapping for one keyboard, I don't need to worry about whether such setting would have some weird behaviour on the other keyboard.  
For example, I have set `8` and `9` on my internal to `(` and `)` and this won't change the behaviour on my TECK.

But in Windows, things are not that happy. I need to keep kicking myself that the remapping won't work on the internal keyboard. This makes it a great pain and inefficient when I need to use the internal keyboard to do some quick tasks. So it makes the laptop not that portable when I can hardly use it without a TECK.

