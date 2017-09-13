---
layout: post
title: "GBA4iOS Update 3: New Features and Changes"
date: 2013-09-17 02:00
comments: true
categories: 
- developer
- GBA4iOS
---

If you've been following my progress on GBA4iOS via Twitter or this blog, you're probably aware that beta testing for version 2.0 has (finally) begun. Out of hundreds of applicants, I had to select only 40; needless to say it was tough. [In my last article](http://rileytestut.com/blog/2013/09/08/the-results-are-in/), I mentioned that I would write up a post shortly detailing exactly how applicants were selected. As I began to write said post, I realized it'd be much better to wait and write about the entire beta testing process as a whole, from selection all the way through the testing process. As such, you can look forward to that writeup after beta testing is completed.

That's not the point of this post, however. This post is for those of you who aren't beta testers; its goal is to keep you updated with what's happening with the development of GBA4iOS. This is the third GBA4iOS 2.0 update post, and this one will focus primarily on two new features I haven't gone into much detail over, and one important change to take note of. These features are small but hopefully appreciated, so I'm glad I get to share them with you!

<!-- more -->

### **Custom Skins** ###

I've mentioned this on Twitter, but I've never truly gone into detail about it. In 2.0, you will be able to download custom skins to GBA4iOS, and switch between them whenever you want. Unlike most implementations of a feature like this, the button layout coordinates are right inside the skin file, so you don't need to import skins then configure the button layout to match it; in other words, it just works. There is no limit to the number of skins you can install, and they can be GBA skins, GBC skins, iPhone skins, iPad skins, portrait skins, landscape skins, and of course any mixture of these. [Paul Thorsen](http://twitter.com/pau1thor), the graphic designer for GBA4iOS, has already come up with some fantastic designs, and they will all be available to download in-app from day one. Here are just a few of the portrait iPhone skins:


{% img ../../../../../images/posts/skins/mario+luigi.png 320 240 %}  


{% img ../../../../../images/posts/skins/retro.png 320 240 %}  


{% img ../../../../../images/posts/skins/squirtle.png 320 240 %}  


{% img ../../../../../images/posts/skins/wood.png 320 240 %}  

As already mentioned, you're not limited to the skins provided in GBA4iOS to download; anyone can create .gbaskin or .gbcskin files and distribute them for others to download and Open In… GBA4iOS, or drag them in via iTunes. Once GBA4iOS 2.0 has been released, I'll write up a tutorial on how to make them (for both Mac and PC), but in the meantime [Mithical](http://twitter.com/mithical), one of the beta testers for GBA4iOS, has posted some of his own designs to his [GBA4iOS beta testing blog](http://gba4ios.mithical.com). Even if you're not interested in the skins, there's some really interesting information there that I haven't mentioned on this site, so you should definitely check it out. 

### **Controller Opacity** ###

An often requested feature, you can now change the opacity of the controller, allowing you to find your own balance between visibility of the game and visibility of the controls. Because not all skins would benefit from being translucent, it's up to the skin designer to flag the skin as such; only then will the skin respond to changes in opacity. For example, the default landscape skin is a simple overlay of buttons on top of the game screen. This is a perfect use case for translucency, so it has been enabled for the skin. However, most portrait skins and some landscape skins are designed to not cover the screen, and as such shouldn't be translucent. Here are some examples of the new customizable opacity:

100%
{% img ../../../../../images/posts/skins/opacity100.png 320 240 %}


50%
{% img ../../../../../images/posts/skins/opacity50.png 320 240 %}


20%
{% img ../../../../../images/posts/skins/opacity20.png 320 240 %}


And even 0% if you choose.
{% img ../../../../../images/posts/skins/opacity0.png 320 240 %}


### **Important Change** ###
Unfortunately, with all this comes some bad news. Because it is much harder to update an app outside of the App Store, I need to make sure version 2.0 has all the features in it I want for the foreseeable future. iOS 7 has included some incredible new features for developers (such as support for game controllers and new networking APIs), and 2.0 takes advantage of all of these. When implementing these features, however, it's important that the app doesn't try to use them in previous versions of iOS, as that would result in a crash. Up until now, I've been careful to do this, but only because these features were easy to exclude in earlier iOS releases. Unfortunately, this has been holding back 2.0 from being the true redesign I aimed it to be. After much debate, I have decided GBA4iOS 2.0 will be an iOS 7 exclusive app. This decision was not made easily, and I know those of you using iPhone 3GSes and iPod touch 4Gs will be disappointed by this, but for the majority of GBA4iOS users this is the best choice. This isn't to say the owners of these older devices are left out in the cold; GBA4iOS 1.6 will continue to be around to be installed on any currently supported device. However, future versions of GBA4iOS will require at least an iPhone 4 or higher, iPad 2 or higher, iPad mini, or iPod touch 5G or higher. Because of this, beta testers should expect to see some nice enhancements in the beta after iOS 6 support is officially dropped, which will probably be in the next week or so. 

On a lighter note, GBA4iOS beta testing has been going really well, and I've already fixed a lot of bugs plaguing the first beta. If it continues to go this well, expect to see GBA4iOS 2.0 released in **October**, just in time for whatever new iPads Apple is planning on unveiling. I know you've all waited a long time for this, and it's finally almost here. Just hold out for (hopefully) one more month, and you'll be able to experience Gameboy Advance on your phone like never before.