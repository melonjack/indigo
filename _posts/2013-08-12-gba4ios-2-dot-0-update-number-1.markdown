---
layout: post
title: "GBA4iOS 2.0 Update 1: Progress So Far"
date: 2013-08-12 00:28
comments: true
categories:  
- GBA4iOS
- developer
---

As I've said before, GBA4iOS 2.0 is a complete rewrite of the original app. What that means is *every* feature in the current version of GBA4iOS has to be rewritten from the ground up for 2.0, and this process takes quite a bit of time. So why do this instead of just simply adding the new features to the existing codebase? The answer is simple: because it's about damn time.

The original version of GBA4iOS was written as a quick hack to get a modified version of gpSPhone to work on non-jailbroken devices. The code was messy, and implementing new features just added to that mess. This worked for when the app was only for developers, but now that everyone is able to download it, this simply isn't good enough. Lots of small annoyances (such as no animation when rotating the device, or the pause menu only being in portrait) exist because of this scrapped-together code, but there are many bigger features that are affected such as the audio skipping. By rewriting the app, I can fix all of these issues, and the app will feel as polished as an App Store app. To keep you guys updated with my progress, I'll post these updates semi-regularly, and I'll try to detail what I've accomplished, what I'm working on now, and any other pieces of information you should know.

<!-- more -->

My first priority for this release is to make the code well structured so it's easy to understand and change later on when I  need to add new features. I'll also be continuing to open source it so any developer is free to fork it and send pull requests.

Secondly, I'm taking full advantage of the new iOS 7 capabilities to give the app just that extra bit of polish. The in-app web browser will return, allowing people to download ROMs without having to leave the app and launch Safari, but this will only be supported on iOS 7 and up. Similarly, there are many small UI enhancements, but again they will require iOS 7 or higher. GBA4iOS will work just fine on iOS 6, it just won't have all these extras.

So far, I've implemented the main core features that take the most time to implement. These include:
 
- Downloading ROMs (In-app browser iOS 7+, via Safari iOS 6+)
- Playing GBA ROMs (don't worry, I'll get to GBC soon.) 
- Controller skins
- Portrait and Landscape support (with rotation animation, finally!)
- Some other secret features

As for what I'm currently working on, in the next week I plan on completing everything in this pause menu:  

![../../../../../images/posts/Pause_Menu.PNG](Pause Menu)

After that, I'll work on the remaining settings, such as dropbox sync. So there's still a lot to be done, but I can assure you I'm working as quickly as I can!





