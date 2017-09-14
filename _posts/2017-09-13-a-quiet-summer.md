---
layout: post
title: A Quiet Summer
date: 2017-09-13
comments: true
category: blog
author: riley
tag:
- developer
- delta
---

As many of you are aware, there haven’t been many updates on Delta for the past few months. This prolonged silence has understandably caused some to [question whether Delta has been cancelled or not.](https://www.reddit.com/r/jailbreak/comments/6yo6zq/comment/dmpq1dt?st=J7BAMEDJ&sh=39eaf05e) Well, today that’s changing. First of all, no, Delta has not been cancelled. I’ve been working on Delta for almost three years now, and have devoted a significant portion of my free time towards completing it; there’s absolutely no chance I would not see this through until the very end.

But why has this summer been so quiet? The answer is fairly straightforward: I’ll be graduating from the University of Southern California this upcoming Spring, which meant this past summer was my last summer before being out in the “real world”. For this reason, the majority of my summer was spent traveling, and time normally spent in front of a computer was instead spent exploring San Jose, San Diego, Austin, Disney World, and even New Zealand.

However, my senior year has now started, so I’m back to a more “normal” schedule. What does that mean for Delta? Basically, I’ll be putting in consistent hours towards finishing it, and that _truly_ is my priority, trust me (just don’t tell my professors). Additionally, now that my schedule is more predictable, I plan on posting updates on Delta far more frequently, whether it be here or on my Twitter account [@rileytestut](https://twitter.com/rileytestut).

So on that note, I have a few announcements regarding Delta that I’m sharing with you all today, with more to come in the near future.

## Open Source

Since the beginning, the plan has been to develop Delta in private, then open source it upon completion. This was to prevent the app from leaking prematurely and having people install buggy, and probably very broken versions of the app, especially ones that could result in data loss. This was the same development process for GBA4iOS, which worked very well for us.

However, Delta differs from GBA4iOS in that it's actually very modular. The app itself is a glorified wrapper around another framework called DeltaCore, which serves as an abstraction over more specific Delta emulation cores. These Delta emulation cores wrap up specific emulator cores into frameworks which are then accessed indirectly via DeltaCore. For example, to emulate SNES games, the Snes9x emulator core is wrapped up in a Delta core (SNESDeltaCore), which Delta controls through the DeltaCore framework. Because of this modularity, it's possible for the components to be developed independently of each other, and as a result each has its own private repo on Github. 

Despite this modularity, all components have been treated as one in terms of what should be considered the app Delta, and as such all have been privately worked on. Starting today, however, this is changing. From now on, the Delta app itself will continue to be developed in private for the aforementioned reasons, but the other components will be developed in the open. Specifically, this includes the DeltaCore framework, and the current fully supported Delta cores: SNESDeltaCore, GBADeltaCore, and GBCDeltaCore. Additionally, N64DeltaCore will be open-sourced once N64 support in Delta itself has been added.

Why have we decided to change this? Primarily, we wanted to have more transparency with the development going on. Often I'll be working on DeltaCore adding new functionality or revisiting unfinished parts of the codebase, but this may result in no visible changes in the app itself, so it may seem like not nearly as much development has happened. Furthermore, this means people can see the daily changes made to the codebase without having to wait for new betas, which are far more spread out.

Additionally, this means developers will be able to look through the codebase and test the code themselves, which may allow them to fix any issues they find, resulting in a more stable codebase for everyone.

**GitHub Repos:**
* [DeltaCore](https://github.com/rileytestut/DeltaCore)
* [SNESDeltaCore](https://github.com/rileytestut/SNESDeltaCore)
* [GBADeltaCore](https://github.com/rileytestut/GBADeltaCore)
* [GBCDeltaCore](https://github.com/rileytestut/GBCDeltaCore)

## Delta Feature Blog Posts

Since not everyone is familiar with Github, or simply doesn't want to follow Delta progress through a sequence of commits, I will also begin writing blog posts detailing different parts of Delta I'm working on, which will give a more high-level overview than the code itself. Such posts may include new features, design decisions, or really anything else that might be worth sharing with everyone!

I hope to release these posts semi-frequently, to ensure there is a steady-stream of information leading up to the actual launch of Delta. So to start, I'm [releasing the first post today](/blog/2017/09/13/delta-features-inputs/), detailing the different forms of input supported by Delta when playing games.

## Distributing Delta

In addition to all the work being put in towards finishing Delta, there is another _huge_ part of the puzzle that hasn’t been publicly discussed much: how will Delta actually be distributed? The way GBA4iOS was distributed has since been patched by Apple, so to get Delta out there to everyone, we’ve been trying very hard to solve this problem.

The good news? We think we’ve figured it out. However, we’re still in the early stages of implementing it, so we’re cautious about saying anything concrete about it since it’s still very possible we come across unanticipated roadblocks. That being said, we’re continuing to work on it, so hopefully soon we’ll have a better understanding of what all will be involved.

Until that point, we’re going to continue to be relatively quiet on this matter, but hopefully the higher frequency Delta updates will make up for this :)

## Next Beta?

So, you might be thinking, it’s been a while since the last beta…_when is the next one coming?_ The answer: in the next few days! The original plan was to release it before before posting these updates, but a last minute issue delayed it by a couple days. Ultimately, I decided it was better to stop waiting to release the beta to publish these updates, since I know people have been getting frustrated. So yes, next beta is coming very very soon! 

As for what’s in it, I’ve rewritten the entire input-handling system to accommodate some of the features highlighted in [the other blog post](/blog/2017/09/13/delta-features-inputs/), which unfortunately took much longer than anticipated. I also have been working on the syncing infrastructure over the summer, and while a significant amount of progress has been made towards completing it, there’s still more to be done before it will be in a beta. Good news though, syncing was the hardest remaining task in Delta, so the remaining features will take far less time 🎉.

## Conclusion

I am genuinely sorry for the lack of updates over the past few months, but now that I’m back to a normal-ish school schedule, I am aiming to be far more open about Delta progress until it is finished. By open sourcing the underlying components of Delta, as well as publishing more blog posts on Delta features, I hope that Delta development will seem like less of a black hole, and more of something that everyone can be keeping up-to-date on.

Finally, thank you all for still being so interested in this project. Seriously, it’s a _lot_ of effort to get everything finished, but it’s very motivating to hear from all of you about how excited you are to play Delta; trust me, we’re very excited for you to play too! We’re slowly approaching the end, but we’re certain it will be worth the wait, so just keep holding on a little bit longer.
