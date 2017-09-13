---
layout: post
title: "GBA4iOS Update 4: What's Left"
date: 2013-10-03 12:32
comments: false
categories: 
- developer
- GBA4iOS
---

Now that October is here, it's time to start wrapping up development on 2.0. For the past month, my beta testers have been tremendously helpful with finding bugs, which means I can focus more of my time on fixing them and implementing new features rather than spend time looking for all possible bugs. So thank you testers, and keep up the good work!

However, while GBA4iOS is reaching completion, there are still some features I haven't implemented yet. It's not that these features aren't coming, but due to one reason or another it made sense to wait to implement them. Since not everyone can be involved in the beta testing process, this post should serve as an update on progress for you all. Just remember: even though they're not implemented yet, the following features _are_ coming, I promise.

<!-- more -->

### **iPad Support** ###

One of the most widely asked for features, I knew I had to do this one right. The most important thing by far was to make sure the button layout allowed for easy access to all buttons, because controls that are hard to use essentially break the app. I've been experimenting with different UIs internally for a while, and I think I've finally come across a design that allows for easy gameplay, while taking advantage of the iPad's bigger screen. In fact, I like the design so much I'm reimplementing many of the same ideas in the iPhone version. Thankfully, since the foundation is already there it shouldn't take too long, so testers should expect iPad support in the next beta, and everyone else should expect to see some nice screenshots and videos soon!

### **Dropbox Sync** ###

There's a reason I didn't choose iCloud for syncing. As awesome as it is, very little control is given to developers over how it actually works behind the scenes. For basic preferences, this is fine; if all hell breaks loose and iCloud breaks, all the user has to do is go back and change the synced settings. However, when dealing with data as sensitive as game saves, it's _very_ important that there is no chance of data being erased. Dropbox gives the power to developers to sync their data how they wish, which means I have full control over when and how game data is synced. This is very important, but it  also means I have to be very careful with how it's implemented. This is why it's not implemented yet; it takes a lot of work to get a completely reliable syncing service. This feature is the one that will push GBA4iOS back the most out of any; if the end of October is approaching and syncing isn't fully reliable, I'll have no choice but to push back the release to finish it. 

### **iOS 7 Controller Support** ###

I'm just as excited as all of you are for true physical controller support in version 2.0, but there's just one problem: no controllers are available yet! The code itself for integrating with these controllers is very easy (thanks Apple!), but I can't do much without having controllers to test with. Just like Dropbox Sync, this is another feature that can potentially push the release back. However, it appears Logitech is preparing to announce one of their own soon, so fingers crossed.

### **Gameboy Color Support** ###

Trust me, I want this implemented as much as you all do. Just like with iPad support, I wanted to make sure I had mostly completed the design of the app and how it works internally before throwing a completely new code base into the mix. This is something it seems a lot of people don't realize: just because the Gameboy Advance plays Gameboy Color games does _not_ mean a Gameboy Advance emulator can automatically play GBC games. They are two completely different systems, so to support GBC games I have to use a completely separate emulator under the hood. Thankfully, because the two emulators I'm using as backends for GBA and GBC ROMs share much of the same code, it won't be as hard as it could be to implement it. To get you excited though, [my graphic designer @pau1thor tweeted a preview of how GBC playback will look](https://twitter.com/pau1thor/status/385114200705495040/photo/1), and personally I think it looks beautiful.

While there are a few smaller features that aren't fully implemented, these seem to be the last four big ones. However, there are still a few surprises I have yet to reveal, and I also plan on releasing something that should get you all pumped for 2.0…but that's for a later date. As always, I'll keep you updated via Twitter and this blog, so keep checking in! 