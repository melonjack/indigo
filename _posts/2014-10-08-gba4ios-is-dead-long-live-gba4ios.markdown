---
layout: post
title: "GBA4iOS is Dead. Long Live GBA4iOS"
date: 2014-10-08 01:01:33 -0500
comments: true
category: blog
author: riley
tag:
- developer
- gba4ios
---

## A Brief History ##

Seventeen months ago, GBA4iOS – our attempt at a Game Boy Advance emulator for iOS – was released. This wasn’t the first time an emulator had been released on iOS; in fact, iOS has had a rich history of emulators finding their way to the platform. However, because of Apple’s somewhat strict (or, as some might say, limiting) guidelines, these apps never had a chance of being approved for the App Store. Rather, they found a home in the far more lenient Cydia store, where users could find and download them as they pleased – assuming, of course, that they had jailbroken their device. While this worked, it severely limited the potential consumer base for the apps; some would be tempted to jailbreak to install the apps, but the vast majority (myself included) felt that jailbreaking required too many compromises for such a minute gain. If only there was a way to install apps not allowed in the App Store (also referred to as “sideloading”)   without having to jailbreak a device first.

That is where GBA4iOS comes in, and why it found so much success despite not being the first (or even necessarily the best) Game Boy Advance emulator for iOS: it was a jailbreak app, but for non-jailbroken devices. But how was this possible? After all, Apple is notorious for locking down their platforms in order to ensure a consistent, safe environment for their users, so how is it that an app like GBA4iOS could be installed on anyone’s device – jailbroken or not – without breaking Apple’s rules?

The short answer is simple: it can’t. We broke the rules.

<!-- more -->

Since iOS (then iPhone OS) 2.0, there have been not one but three official ways to distribute apps to users: the App Store, which required Apple to review and approve your app manually; Ad Hoc distribution, where you could send pre-release versions of your apps to up to 100 registered devices; and last-but-certainly-not-least the Enterprise program, where you can distribute apps internally to as many devices as you wanted. Because Apple would never allow GBA4iOS into the App Store, and because we knew 100 devices wasn't nearly enough, we opted for the third option. Of course, we always knew at any time Apple could shut down distribution of GBA4iOS by revoking our signing certificate (all apps on iOS have to be "signed" in a secure manner in order to be run to prevent malicious apps from being installed), but we decided it would be worth it so people could enjoy playing their old Game Boy games on their phone, even if it was just for a little while.

The truth is, we didn't anticipate the level of popularity GBA4iOS reached. At first it was still relatively obscure – we did zero marketing since it was more of a hobby app, and we knew it was only temporary – but soon enough more and more people began finding out about it, and within a month the app was making headlines. Naturally, of course, this increased awareness of the app reached Apple, and within a day of GBA4iOS reaching peak popularity, Apple revoked our signing certificate, and GBA4iOS was dead.

Or so we thought.

If there's one thing you can count on, it's that people who want to play Game Boy games on their phones will try almost anything to accomplish this goal. And sure enough, one crazy enough idea turned out to work, and that trick is why I'm writing this blog post today. Colloquially referred to as the "Date Trick", it was discovered that by setting the date of the device back a day, certain security checks in launching GBA4iOS would fail, and allow it to be installed. It seemed like such a crazy idea, but it worked, and that's all that mattered. 

Fast forward eight months, and we release [GBA4iOS 2.0](http://gba4iosapp.com), a complete rewrite of the original app. Now that we knew about the Date Trick, we were motivated to give the app every bit of polish it deserved. No longer was it a hobby intended to be used by a few people; it was now being used by millions of people worldwide. Sure enough, less than thirty minutes (!!) after we released GBA4iOS 2.0, Apple revoked our new certificate once again, but all that did was force people to set the date back to install the app; an inconvenience for sure, but far easier than jailbreaking the device. We've continued to update the app since, and it's survived several iOS updates since then – such as 7.1 and 8.0 – none of which have prevented the Date Trick from working.

Of course, that ends with iOS 8.1 when it is released later this month. When the first beta was released just over a week ago, it appeared that the Date Trick no longer worked. Not wanting to jump to conclusions, we opted instead to see whether the second beta kept these changes (even though from the device logs it seemed pretty clear this change was intentional). Unfortunately, with the release of the second beta of iOS 8.1, it does seem that the Date Trick is no more.

GBA4iOS is dead. Again.

## What Happens Now? ##

If you're reading this blog post, there is probably one question you want to know more than anything: "is there a future for GBA4iOS?" As with most details surrounding GBA4iOS, that answer is not entirely straightforward, but I'll do my best to answer it.

As of iOS 8.1, you will no longer be able to download GBA4iOS, or any other apps which require the Date Trick to be installed. Any attempts to will result in the app downloading, but failing to install due to iOS recognizing the invalid certificate. Similarly, and perhaps most unfortunately, _already installed apps that require the Date Trick to work will no longer open_ even if you do set the date back. If you are running iOS 8.1, you will be unable to install or play GBA4iOS.

That is, with one exception. From the beginning, GBA4iOS has been open sourced, meaning that all the code needed to make the app has been available online for anyone to download. If you are a developer, or if you are simply a member of Apple's paid developer program, you can download the code yourself and install onto your own device, without having to set your date back or anything. Previously, the code was hosted on GitHub, but due to [some legal issues](http://rileytestut.com/blog/2014/05/18/what-is-going-on-with-gba4ios/), it is now being hosted on [Bitbucket](https://bitbucket.org/rileytestut/gba4ios/). To install, simply download the code and follow the instructions in the README; once you've done this, you should be able to run the app on your device.

## What Happens Down the Road? ##

GBA4iOS will continue to be maintained, and we'll also continue to release controller skins and Event Distributions (we have some really awesome events lined up, trust us). We'll do our best to offer support for the app, with one caveat: we'll officially be shutting down the support@gba4iosapp.com email. We were already having trouble keeping up with the insane amount of emails we were receiving, and with GBA4iOS effectively dead it doesn't make sense to keep it around. That being said, we'll do our best to answer any questions you have on Twitter. I'm [@rileytestut](http://twitter.com/rileytestut), and my incredibly talented partner and graphic design artist Paul Thorsen can be found under the username [@pau1thor](http://twitter.com/pau1thor). We want it to be clear we are _not_ abandoning GBA4iOS, and will continue to update it so that it works on future versions of iOS, even if it can only be installed by compiling it yourself.

Some of you may be asking, “what about GBA4iOS 2.1?”. We’ve been promising that we’d release a big update to GBA4iOS that includes the much anticipated multiplayer feature, allowing GBA4iOS to communicate wirelessly with other devices running GBA4iOS to enable multiplayer features such as trading Pokemon, and we’re happy to say that this has not changed. However, now that we know we have limited time before iOS 8.1 is released, we’re opting to do something I originally said I would not do: we’re going to release GBA4iOS 2.1, but with multiplayer functionality in beta. 

<blockquote class="twitter-tweet" lang="en"><p>I should probably write up a blog post, but here&#39;s the gist: I will not release an inferior product. Period.</p>&mdash; Riley Testut (@rileytestut) <a href="https://twitter.com/rileytestut/status/513905976244592643">September 22, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

This means that it will be functional, but not running at full speed, and with potential connection instabilities. Under normal circumstances, I’d much rather hold off on the release of the update until I had completely polished it, but right now our priority is to get the update out before iOS 8.1 drops for everyone.

So good news is GBA4iOS 2.1 is now coming sooner than originally intended. But we’re not stopping there; because we want to test the app as much as possible before releasing, we’ll be open sourcing the code for 2.1 tomorrow, October 9, allowing anyone with a developer account to install and test it for themselves. Because this is still a beta, we’re not including multiplayer in this first release; that will come soon after we finish the UI and ensuring it at least works well. But all other features - such as selectable color palettes for original Game Boy games, ability to set a homepage for the web browser, and full iPhone 6 and 6 Plus support - will be working as intended.

For GBA4iOS 2.1, we’ll also be adding a new distribution method that’s been heavily requested: for the first time, GBA4iOS will be able to be installed officially from the Cydia store. For those who are jailbroken, this means you will be able to install  and use the app without having to set the date back, which should be much simpler and more pleasant. Plus, if/when an iOS 8.1 jailbreak comes out, the app will still work. We’ve been hesitant to do this before - GBA4iOS has and always will be a primarily a non-jailbroken app - but due to the circumstances we feel now is the time to change our stance.

## Apple is Not to Blame ##

To be clear, we are not blaming Apple for “purposefully” trying to kill GBA4iOS, and neither should you. Not only did we violate our developer agreement with Apple, but we were _exploiting a security issue in iOS_. Of course this was coming, it was only a matter of time. And yes, it sucks for all of us that wanted to be able to play our classic games on our iOS devices, but there are [other platforms for that](http://www.android.com), as well as, of course, official Nintendo hardware platforms (which by all accounts you should own if you’re playing these classic games in the first place!). There’s always a chance Apple will allow official sideloading of apps in the future, but I wouldn’t count on it happening any time soon; that’s a discussion for another day.

You can be assured that if any other distribution method pops up that would allow people to install GBA4iOS on non-jailbroken devices, we’ll go for it. Despite knowing GBA4iOS’ time was limited, we still put our heart and soul into it to make it the best app it could be. It’s easy to accept this as the end, but we’ll be treating it as a temporary hiatus. The moment it becomes possible for GBA4iOS to return, it will, and (hopefully) with Apple’s blessing.

## Future Projects ##

With GBA4iOS reaching the end of its current lifespan, we’ll be moving on to our next app, Hoot, and we are happy to say it will be distributed officially through the App Store. After dealing with all the workarounds needed to distribute GBA4iOS, it’ll be nice to return to the relatively “simple” (comparatively) life of an App Store developer, even if it means having to deal with Apple’s infamous approval process. In addition, we’ll be able to take advantage of some nice iOS features such as extensions and iCloud, which were unavailable to us due to how we were distributing GBA4iOS, and we have some great ideas lined up. As always, we’ll reveal more about Hoot as we get closer to release, which should come much sooner now that we can spend all of our time on it. 

To wrap-up, yes, iOS 8.1 kills GBA4iOS. We’ve always known the day would come when this would be the case, but now that it’s here it’s still sad for us, as I’m sure it is for many of you. However, we’re not saying this is the end forever; we’ll still very much be maintaining GBA4iOS and allowing it to live on as an open-source project, and should the day ever come where we can distribute it once again, we will. For now though, we’ll release GBA4iOS 2.1 with a beta implementation of multiplayer, and then begin working on finishing our next app Hoot. If you wish to stay involved in our development on GBA4iOS and future apps, you can [follow me on Twitter](http://twitter.com/rileytestut), or [my partner Paul Thorsen](http://twitter.com/pau1thor).

Finally, thank you for downloading and enjoying GBA4iOS; we’ve only ever done this so people can feel the joy they once felt playing these classic games for the first time, and I’m glad we succeeded!


