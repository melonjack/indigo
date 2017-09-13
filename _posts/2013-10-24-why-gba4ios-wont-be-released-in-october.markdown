---
layout: post
title: "Why GBA4iOS 2.0 Won't Be Released in October"
date: 2013-10-29 12:32
comments: false
categories: 
- developer
- GBA4iOS
---

[Two blog posts ago](http://rileytestut.com/blog/2013/09/17/gba4ios-2-dot-0-update-3-new-features-and-changes/), I mentioned that if all went well, I hoped to have GBA4iOS 2.0 released by the end of October. I was hesitant about writing this, but I knew that everyone wanted an ETA, so I went ahead and put it in. However, that's all it was ever meant to be — an estimate. Unfortunately, it seems as this information spread from person to person, the estimation part was left out, and instead my estimation became a promise. For that, I am sorry. I had full intentions of releasing the app by the 31st of this month, but I now see this was (slightly) too ambitious a goal. Besides dealing with the problems that come up with developing an app, I have to also make time for school and work, among other things (hell, I have to finish a college application by next Friday). 

Before jumping to conclusions, this does not mean development of 2.0 has stopped; I'm very much still working on it, and have been for the past few months. But before I get into more details over why GBA4iOS has been slightly delayed, there is one question I've been asked many times that I need to address: why don't I just release a version now and update it later? It's a reasonable question, considering App Store apps do it all the time, and it would allow people to play GBA4iOS 2.0 sooner. To be completely honest, I would love to do this, but it's just not possible. I've avoided answering this question for a while because I didn't want to get into the technical reasons, but since GBA4iOS will no longer be finished in October the least I can do is give you insight into why I'm waiting until 2.0 is 100% complete before releasing it.

<!-- more -->

For an App Store app, installing onto a device is easy; iOS is designed to allow 3rd party apps from the App Store to be easily installed updated. To get into the App Store, an app must survive the Apple's App Review Process, an infamously stringent process every app undergoes to make sure it is safe, useful, and legal. Understandably, GBA4iOS would never be allowed in the App Store, due to the gray legal area emulators reside in. Instead, the original version of GBA4iOS was distributed outside the App Store using something called an Enterprise Certificate. Even though this is normally used by bigger companies to install their own custom apps on their employees' devices, there is no technical reason why it couldn't be used for any app to be installed on any device. As such, this is how GBA4iOS was able to be installed from outside the App Store, and remains the reason you can still download it. 

Since this is breaking Apple's enterprise rules, however, they revoked the certificate on July 17 of this year. I won't go into the technical details of code signing, but basically this meant I was unable to release any more updates to GBA4iOS. While it was eventually figured out that setting the date on the device back to before the day Apple revoked the certificate allowed GBA4iOS to continue to be installed, this had no effect on being able to release new versions; I was still stuck.

GBA4iOS 2.0 will use a similar distribution method. For a short period, you will be able to install 2.0 quickly and easily without having to set your date back. However, inevitably Apple will shut down this method as before. This is why I can't hold an open beta or release an incomplete version; _once I release GBA4iOS 2.0, I will be unable to update it_. That's why 2.0 is such an ambitious release. Since I won't be able to update it, I need to future proof it for the foreseeable future. Now, this doesn't mean the app will _never_ be updated, but it means you shouldn't expect one for some time. Basically, if I chose to hold an open beta or pre-release the app, you'd have to wait upward of months for the other features to come, instead of a few more weeks.

Hopefully, now you can see why I've been so adamant about keeping the beta testing closed. I get one shot at releasing 2.0, so I need to make sure everything is perfect. Unfortunately this takes time, but in the end it'll be worth it. Since this post is unfortunate news for you all, I think the least I can do is share with you what's keeping GBA4iOS from being released this month. 

### __GBC Support__ ###

Currently, I have GBC support working just fine in GBA4iOS. However, there's one problem: the app can either only play GBA games or GBC games, but not both. I have to choose whether I want to use GBC code or GBA code when I make the app, as when I try to do both at once the app errors out. This is because of how both code bases are designed: they share much of the same code — which makes it easy to port features such as save states and cheats over to GBC — but it also means when they're both in the same app (which they were never intended to be), they essentially fight for control. To fix this, I have to go in and change all this shared code to determine whether to use the GBA or GBC emulator depending on which ROM is loaded. Easy? For the most part, the logic is pretty simple. Does it take a long time? You betcha. Thankfully, I'm down to the last few code changes, so it should be finished soon. This was by far the feature that took the longest to implement, and it's finally almost done.

### __iOS 7 Controllers__ ###

I was really hoping some more information would be revealed about the release of controllers by now. This is actually a very easy feature to implement; the problem is having to code it without testing it. I know this is a top requested feature, and trust me I want to use Bluetooth controllers as much as you. However, I've delayed the release of GBA4iOS 2.0 enough, so unless a controller is released in the next two weeks. I'll just have to do my best to code for every possible scenario (controller dying, being disconnected, second controller connecting, etc.). Unfortunately there's not much more than that I can do.

### __Wrap Up__ ###

To summarize: GBA4iOS 2.0 will not be released in October. I shouldn't have posted an ETA, and I won't be posting one this time, so please don't ask me. From a developer standpoint, the app is very close to being completed, but that's all I'll say. I'm very sorry. I know many of you were looking forward to playing your GBA and GBC games on this new version this month, but you'll just have to hold out a little bit longer. I get one shot at releasing 2.0, and I need to make sure I do it right. 

Thanks for understanding, and I promise GBA4iOS 2.0 will be worth it; I still have some secrets up my sleeve.


