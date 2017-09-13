---
layout: post
title: "GBA4iOS 2.0 Update 2: Pause Menu"
date: 2013-08-20 11:05
comments: true 
category: blog
author: riley
tag:
- developer
- GBA4iOS
---

As you may know if you've been following me on Twitter, I've been on vacation in Los Angeles for the past few days. [I met a girl (kinda)](https://twitter.com/rileytestut/status/368914755269849088/photo/1), stayed with my sister at USC, and of course spent some time at the beach. However, while it may not have seemed like it when going through my Twitter timeline, I managed to work on GBA4iOS in my spare time. There's some nice stuff I want to show off; hopefully you'll find it all great as well.

Last week, [I said my goal was to be finished with everything in the pause menu](http://rileytestut.com/blog/2013/08/12/gba4ios-2-dot-0-update-number-1/), so that's exactly what I did. As a recap, here's what the pause menu will look like:

![Pause Menu](/assets/images/posts/Pause_Menu.png)

While I may add features to the menu, these current ones will all definitely be in the release of 2.0. Most of these have been in previous versions of GBA4iOS, but they've all been tweaked enough that they're worth detailing again.

<!-- more -->

### **Return To Menu** ###

Returns to the GBA4iOS main menu. Nothing too groundbreaking here, but there is a nice tweak to the behavior. Whereas previously this would quit the current ROM, now it simply pauses it and keeps it suspended in the background, à la iOS multitasking. This means you can exit to the menu, then open the ROM again and be just where you left off. If you've ever played with [nds4ios](http://nds4ios.angelxwind.net), you'll be used to this.

### **Fast Forward** ###

The ability to speed up the ROM never really had an official name in the old versions of GBA4iOS, the option to enable or disable it was simply titled "Toggle Speed". This functions exactly the same as the previous implementation, but I've renamed it to something that actually makes sense, especially since this is what other emulators are calling this feature. So yeah, magic.

### **Save/Load States** ###

Again, the basic functionalities of these two options remain the same, but I've added some features that should make them much better to use. See if you can spot all that's new in this screenshot:

![Save States Preview](/assets/images/posts/Save_States_Preview.png)

Awesome right? But just in case anything needs clarification, here's all that's new:  

- Ability to rename save states, since "World 8-1" is much easier to remember and understand than Aug 13, 2013, 5:27 PM.  
- Unlimited number of save states, so you don't have to worry about which ones you can overwrite and which ones you want to keep.  
- Speaking of keeping save states, you can now protect them. By renaming a save state, it automatically protects it for you, meaning you cannot overwrite it with a new one. You can, however, delete a protected save state if you no longer want it.

### **Cheat Codes** ###

Ah cheats, the number one most requested feature since version 1.0. Yes, finally, they are coming in 2.0, and they'll be incredibly easy to use. There will be no need for a master code, and you won't have to split up multi-line codes into multiple cheats. Also, you'll be able to add, remove, enable, and disable cheats on device without having to exit the ROM. Just be wary of using cheats; games were not made to be used with them, and may have unintended side effects as a result. If you mess up a game with cheats, there is nothing I can do, so just be careful.

![Cheats Preview](/assets/images/posts/Cheats_Preview.png)

### **Sustain Button** ###

This is actually a feature I made for SNES4iOS, but it never really worked too well, and it was a bit confusing. As with everything else in 2.0,  I've rewritten it to be easy to use and work well.  But what *is* the feature? Simple: it holds down a button for you so you don't have to. This is very useful in games like Super Mario Bros. or Pokemon when you need to constantly hold down the B button to run, or in Mario Kart when you need to hold down A to keep your vehicle's engine running. 

### **One more thing…** ###

As I mentioned yesterday on Twitter, if you're playing one of the main Pokemon games you'll have another option in the menu:

![Event Distribution Preview](http://rileytestut.com/images/posts/Event_DIstribution_Preview.png)

This is one feature you just *have* to try out, so I'm not planning on giving too much away until 2.0 is released. However, I will say a few things:

- Akin to the Nintendo Pokemon Events, you'll be able to get rare items via this option for your game.
- Unlike the Nintendo events, this is not limited to the in-game event items such as the Aurora Ticket.
- This also does *not* use any cheat codes.

These new features and improvements have really made 2.0 so much more fun to use, and I can't wait to wrap everything up so you all can enjoy it. However, since this is a *complete* rewrite, I'll need some help testing the app to make sure there aren't too many bugs. If you're interested in helping out, stay tuned – I'll have more info shortly!




