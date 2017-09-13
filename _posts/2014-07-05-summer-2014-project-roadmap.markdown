---
layout: post
title: "Summer 2014 Project Roadmap"
date: 2014-07-05 17:06:43 -0500
comments: true
categories: 
- developer
- gba4ios
- hoot
---

About a month ago, I graduated from high school. While I've been enjoying my time off and being social with friends (we only have a few months left before everyone leaves for college!), I certainly have been hard at work on not only GBA4iOS, but also a new app we call Hoot. However, between coding and spending time with friends, I haven't taken much time to actively talk about what exactly was happening behind the scenes, and what you should look forward to seeing in the next few months. As such, I've decided to write this blog post outlining the project roadmap my team and I have in place for the summer, so you know exactly what is coming when and what to get excited for! Of course, everything here is just a plan; there are no guarantees as to the release date of anything, but we're confident enough in our plans to give you our thoughts.

<!-- more -->

## GBA4iOS ##

There should be no surprise that updates to GBA4iOS comprise a big portion of my app development time, especially because we're working on two future versions simultaneously. The first of which, GBA4iOS 2.0.5, is a smaller update, mostly to officially support iOS 8, while including a few notable features. Once this is complete, the next update will be 2.1, a massive update featuring the most-requested feature of all: multiplayer. To better explain what is happening, I've divided this section up into two—one for each update—and focus on not only the new features, but what hurdles stand in the way and estimated release dates.

**GBA4iOS 2.0.5**

About a month ago, Apple unveiled iOS 8, and brought with it a multitude of new features everyone should be excited about. Unfortunately, along with these new features comes a lot of changes to the underlying features used to make apps, such as GBA4iOS. Because of this, some things are quite broken when playing GBA4iOS on iOS 8, and it is our primary focus right now to fix these bugs. While we intended for this update to be released a while ago, in iOS 8 beta 2 some very important features needed by GBA4iOS were not working properly (especially on iPads), so we weren't able to release the update. We've filed bug reports with Apple, and from our initial testing of iOS 8 beta 3 it seems many of these issues have been resolved, allowing us to push the update out sooner rather than later.

Besides iOS 8 compatibility, we're also including a new feature that has been long requested - push notifications. No longer will you have to worry about missing Event Distributions, or keep checking to see if there's an update to GBA4iOS; your phone will automatically tell you! This feature will work on both iOS 7 and iOS 8 devices, so you don't need to feel like you need to update to iOS 8 now to take advantage of this feature (as some people had speculated). However, there _will_ be an iOS 8-only Easter egg in this update that will be removed in 2.1, but we won't say what it is. You'll just have to try to figure out what it is yourself :)

As for a release date, expect this one to come out soon, and in the meantime I'll be sure to update you all [via Twitter](https://twitter.com/rileytestut). Of course, what good is an update with push notifications if we don't also put out an Event Distribution shortly after? The promised FireRed and LeafGreen event from before the [Nintendo DMCA takedown notice](http://rileytestut.com/blog/2014/05/18/what-is-going-on-with-gba4ios/) will finally be released, so get excited for that!

**GBA4iOS 2.1**

Of course, this is the update everyone is waiting for. For this update, we've radically updated the look of included controller skins, added the ability to change the color of original Gameboy Games, and of course added multiplayer capabilities. No doubt about it, this is the first "big" update to GBA4iOS 2.0, and we're working hard to make sure it lives up to that name.

Multiplayer has long been in the works; I [tweeted an initial teaser photo of trading Pokemon a little over two months ago](https://twitter.com/rileytestut/status/454318993063432192). So what has been happening in the meantime? Well, despite having it working back in April, it was abysmally slow; so slow that it took well over five minutes to complete a trade (which typically takes around thirty seconds). Since then, I've worked hard on optimizing it and now have it running much faster than before. It now "only" takes 2 minutes to complete a trade, which is more than twice as fast as it was before, yet still 4 times slower than normal. Unfortunately, it seems this is as fast as the current implementation of multiplayer will allow; at this point the bottleneck is hardware, not software. Because of this, we've began restructuring the multiplayer logic to accommodate these bottlenecks, but this is taking some time to get right. 

Right now, we're aiming to only emulate the link cable, and only via local bluetooth/WiFi-Direct. Later down the road, we plan to add full emulation support for the wireless adapter, which could possibly lead to even greater speed improvements for the games that support them (such as the later Pokemon games). As for linking with others over the internet, we very much want to add this capability later, but it may prove to be impossible due to too much latency. However, we'll do our best to make it possible.

Because of the restructurings needed to fix the speed issues, we're aiming to release 2.1 by the end of the summer. Of course, this could change as we find multiplayer easier or harder to implement, but we feel this is a reasonable guess as to when it'll finally be complete. I also plan to start tweeting more about this update as we get closer to its release, so as always stay tuned!

## Hoot ##

GBA4iOS is no longer the only app in development by my partner Paul and myself, and we're going all out on our next app, Hoot. We've added our good friend [Michael Metzger](http://twitter.com/mikemetzger13) to the team, and even have a new teamname for ourselves: [TMT Projects](http://twitter.com/tmtprojects). As mentioned in my [self-documentary](http://youtu.be/BtWjjbei-vE), Hoot has been in development for a little over a year, but was pushed aside in order to focus solely on GBA4iOS 2.0. Now that 2.0 has finally been released, we've resumed work on Hoot, and are hoping to have it released by the end of the year. 

What is it exactly? Well, we're not quite ready to reveal that yet, but we can say it has absolutely nothing to do with emulation or games whatsoever. Unlike the non-jailbroken emulator market, we're preparing to enter a market rife with competition, so we need to be firing on all cylinders to ensure we can compete with some truly remarkable apps (some of which have been so groundbreaking that Apple has borrowed some UI mechanics and put them in their own apps). Of course, that isn't to say the app will feel completely different than GBA4iOS—it will be made by the same people after all, and we want to have a consistent feel between our apps—just don't expect it to play games, that's all. More information will be coming shortly after finishing the updates we have planned for GBA4iOS, so I'd recommend following [@hoottheapp](http://twitter.com/hoottheapp) on Twitter to ensure you don't miss anything!

## A Note About T-Shirts ##

Recently, we [ran a campaign on Teespring](http://teespring.com/gba4ios) selling official GBA4iOS T-shirts. People have been asking us to sell shirts for a while, but I had always been hesitant towards the idea; I thought it would be better to simply focus on the app rather than selling merchandise. However, we did ask for opinions on the matter, and people overwhelmingly said they wanted one and would buy one if they were put up for sale. Because of this, Paul and I decided to run an experiment: we'd have a limited sale of T-shirts, and if we managed to reach our sales goal, we'd know that people would actually be willing to purchase the shirts (instead of just saying they would), allowing us to explore much more expansive options for selling shirts, and possibly other GBA4iOS merchandise. 

However, as you probably know, we didn't come close to our goal; we needed 200 shirts to be reserved before they would be printed, but only 33 were. From this, we decided selling GBA4iOS merchandise would not be a viable option right now; it would take quite a bit of effort to set up, and at this point it doesn't seem the interest is high enough to justify it. This doesn't mean that there will never be GBA4iOS merchandise for sale, but with our primary focus on building apps right now, don't expect to see it for a while.

## Wrap-Up ##

It may be summer vacation, but that doesn't mean we've halted development of our apps in any way. We have some significant updates planned for GBA4iOS, and as they roll out we hope they will make your emulation experience even better than it is now. And while we'll certainly be working on future updates for GBA4iOS beyond 2.1, we also have a brand new app in the pipeline, bringing over what we've learned by making GBA4iOS and applying it to a completely new category of apps. We can't wait for you to see what we've been working on, and hopefully this blog post has given you a small insight into what's happening behind the scenes to bring these apps to you. As always, you can follow [me](http://twitter.com/rileytestut), [Paul Thorsen](http://twitter.com/pau1thor), and now our new teammate [Michael Metzger](http://twitter.com/mikemetzger13) for more news and updates, and for those fellow students out there, keep enjoying your summer vacation!
