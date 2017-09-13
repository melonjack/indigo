---
layout: post
title: "GBA4iOSApp.com, Current Progress, and Future of GBA4iOS"
date: 2013-12-29 16:00
comments: false
category: blog
tag:
- developer
- GBA4iOS
- gba4iosapp.com
---

Wow, I can't believe it's been two months since my last blog post. This doesn't mean I've stopped development of GBA4iOS; in fact, quite the opposite. It just means that between developing GBA4iOS and school work, I haven't had time to sit down and write up a post over the state of 2.0. I've posted bits and pieces of progress on Twitter every now and then, but now that development has begun to wrap up, I think it's time for another post to keep you all updated. Since there's a lot to talk about since the last post, I've divided this one up into multiple parts (as evidenced by the title). If you came here only to learn about release information, you only really need to read the Future of GBA4iOS section, but I'd recommend reading everything since there's some tidbits I haven't mentioned before. 

<!-- more -->

## GBA4iOSApp.com ##
If you've been following me on Twitter, chances are you already know about [GBA4iOSApp.com](http://gba4iosapp.com). But what exactly is it? Well, once GBA4iOS 2.0 is finally released, this will be the central place for all things GBA4iOS-related, and it'll also be the only official place you can download 2.0, as well as 1.6. But why would you want to install version 1.6 over 2.0? As I've mentioned before, 2.0 will be _iOS 7 only_, meaning those of you who can't (or have yet to) update to iOS 7 will be unable to install it. However, even if you're running iOS 7, while normal save files can be transferred to 2.0, save states unfortunately can not. So, if you want to keep using your old save states, you'll need to keep using the older version. As an added bonus, the old version will be (slightly) updated to allow it to be installed alongside other emulators (such as [nds4ios](http://nds4ios.angelxwind.net)).

So eventually, [GBA4iOSApp.com](http://gba4iosapp.com) will have everything you need to download and install GBA4iOS. Right now, however, the site is still very much being worked on. If you loaded the site up right now, you'd see two pages to choose from: Home and FAQ. On the home page, you'll find a trailer for GBA4iOS 2.0, showcasing many of the new features in the update. Expect more trailers as the 2.0 launch gets closer, because there are far too many new features to mention in only one trailer.

On the FAQ page, you'll find a FAQ similar to the one that used to be on this site, but updated to help with both GBA4iOS 1.6 and 2.0. As always, make sure to check there first to see if your questions have already been answered (it'll be quicker for both you and me, trust me), but if they're not there, you can ask [Alyssa Surowiec](http://twitter.com/alyssasurowiec), who is more than happy to answer any remaining questions you may have. 

## Current Progress ##

So, where I do start? Since the last blog post, I've implemented a slew of new features, including Dropbox Sync, Fast Forward, iOS 7 controller support, downloading skins in-app, URL scheme support, splash screens, and brand new controller skins for both iPhone and iPad. Since it's hard to explain these all in only a few paragraphs, I'll highlight a few of them that most people will use and enjoy:

### **Dropbox Sync** ###
Honestly, this feature is the reason that I haven't posted much on this site recently. I started work on it two nights before I wrote the last blog post exactly two months ago, and it wasn't feature complete until only about a week ago. Hopefully everyone will use this feature; even if you don't have multiple devices, it can't hurt to have your data backed up somewhere else in case something happens to your device. 

But how exactly does it work? 

Basically, from GBA4iOS, you can turn on Dropbox Sync, which will begin an initial sync. This initial sync is used to compare the files you have locally with any that already exist in Dropbox, and then uploads/downloads whatever is needed to keep everything in sync. However, there is one safety precaution: if there is already a save file in Dropbox for the game you are trying to sync, as well as a local save file, the initial sync will mark it as conflicted, and will turn off syncing for that particular game. Why mark it as conflicted? Because for the initial sync, GBA4iOS has no way of knowing whether you'd prefer to sync your local save or Dropbox save, so it leaves it up to you to decide. After you decide, GBA4iOS will sync data for that game normally again.

![Dropbox Sync](/assets/images/posts/features/dropbox_sync_overview.png)

How you do resolve the conflict though? From the Dropbox Sync menu, select the game you want to no longer be conflicted. You'll be presented with a detailed syncing view of the game, showing your local save states and any you have in Dropbox. To turn syncing back on, you'll need to select either your local save or any of your Dropbox saves to sync to all your devices. Once you've selected the save you want, toggle the switch at the top to ON, and syncing will resume normally for the game.

![Dropbox Sync](/assets/images/posts/features/dropbox_sync_detail.png)

In addition to save files, cheats and save states are also synced across your devices. This is especially convenient when you get a new device; turn on Dropbox Sync, and just like that you'll have all your saves, save states, and cheats. Plus, at any time you can access these files from the Dropbox folder on your computer, if you want to use them on a desktop emulator (such as the incredibly awesome [Open Emu for Mac](http://openemu.org)). 

### **iOS 7 Controller Support** ###

In the time since the last blog post, two iOS 7 controllers were finally released: the [Moga Ace POWER Controller](http://www.mogaanywhere.com/ace/) and the [Logitech Powershell Controller + Battery](http://gaming.logitech.com/en-us/product/powershell-controller-and-battery). This meant I could finally add the code needed to get everything working, and now that I've finished, I can say that playing Gameboy games using these controllers is fantastic. However, there is one problem: all iOS 7 controllers have their A and B buttons flipped compare to a real Gameboy Advance. Typically, the A button is located above and to the right of the B button, like in the default controller skin:

![Wario Ware: Twisted](/assets/images/posts/features/wario_ware_twisted.png)

On iOS 7 controllers, A is the button on the bottom and B is to the top right. To fix this, there is a menu in GBA4iOS that allows you to customize what each of the lettered buttons does by tapping each one individually and selecting from a list of actions, or by touching and dragging the button actions around. Here are the default button mappings:

![iOS 7 Controller Customization](/assets/images/posts/features/external_controller_default.png)

However, to make the controls feel more akin to a real Gameboy Advance, I've modified these controls for my personal use:

![iOS 7 Controller Customization](/assets/images/posts/features/external_controller_customized.png)

As you can see, I've also mapped the L2 and R2 buttons to Sustain Button and Fast Forward, respectively. This is one of the benefits of having a controller with the extended button set, such as the Moga Ace POWER. Gameboy Advance games only use one set of shoulder buttons, so while by default GBA4iOS uses the second set to act as another pair of L and R buttons, I'd definitely recommend using them to perform the actions I've selected. This is especially convenient because when using Fast Forward via the controller, it starts fast forwarding when you press down and stops when you lift up, similar to how desktop emulators do it.

### **URL Scheme Support** ###
This is a rather new addition to GBA4iOS, as it was only recently suggested to me. However, I'm glad it was, as it's actually quite powerful. Similar to other apps, you can now open GBA4iOS via the gba4ios:// URL scheme. What does this mean? Basically, it means other apps such as Safari and the well-known Launch Center Pro can launch GBA4iOS. Even better, you can launch specific games by configuring the URL scheme. For example, if you had GBA4iOS 2.0 right now, tapping [this link](gba4ios://POKEMON%20EMER-7b058a7aea5bfbb352026727ebd87e17) would open GBA4iOS and launch Pokemon Emerald - even if it's titled something different in your app - if you have the game. If you don't have the game, it'll just open the app.

As mentioned above, this allows GBA4iOS to work hand in hand with [Launch Center Pro](https://itunes.apple.com/us/app/launch-center-pro/id532016360?mt=8), an app used to launch other apps and perform actions. Since the URL scheme allows you to launch any game you have downloaded, you can create a folder in the app and use it as an alternative to the GBA4iOS game launcher. Even better, using [Apple Configurator](https://itunes.apple.com/us/app/apple-configurator/id434433123?mt=12) or something similar, you can add Web Clips to your actual home screen you can tap to launch games. Personally, I have one set up to launch Pokemon Emerald.

![GBA4iOS Web Clip](/assets/images/posts/features/gba4ios_web_clip.png)

### **Surprise: Wario Ware Twisted support!** ###
Well, I kinda spoiled the surprise [yesterday on Twitter](https://twitter.com/rileytestut/status/417105951775133698), and  again with the screenshot of the game earlier in this post, but a brand new feature coming to GBA4iOS 2.0 is support for Wario Ware Twisted. While technically the game has always run, it's been impossible to play since it requires use of an external hardware motion detector. Many of you have asked for the ability to use the iPhone's motion sensors to emulate this hardware adapter, and so 2.0 will do exactly this. It's actually quite fun to play the game on an iPhone, since it feels like an actual iPhone game. So if you're a big Wario Ware fan, be excited!

![Wario Ware: Twisted](/assets/images/posts/features/wario_ware_twisted_shave.png)

## Future of GBA4iOS ##

Development is wrapping up, and at this point I'm mostly fixing bugs. However, there is something important to know about the distribution method: _it is not ready yet_. While I am in charge of development of GBA4iOS, I am _not_ in charge of the distribution method. I am collaborating with other developers to get everything worked out (especially with the changes Apple has done to downloading apps over the air in iOS 7.1), but ultimately the release is not up to me. If I finished the app tomorrow, _I would still not be able to release it_. iOS is made to have apps installed through the App Store; going into this, I knew it wouldn't be easy. Thankfully, it doesn't appear that the distribution method will take too long to finish, but that is why I cannot give an estimate on the release of GBA4iOS. The second I can release 2.0, I will.

On a more exciting note, there is a feature I've started to work on that, while it won't be in 2.0, has a very good chance of appearing in a future version. After cheats, it has been the most requested feature by far, and I can't wait for it to be finished. Without further adieu, I pre-announce a new feature in GBA4iOS:

**Multiplayer Support**

Soon, you will be able to connect different devices running GBA4iOS wirelessly to emulate the Gameboy Advance Link Cable support many games have. This means you'll be able to trade and battle in your Pokemon games, work together in your Legend Of Zelda: Four Swords adventures, and anything else you can do with a link cable. Since it's very early in development, I can't say too much about how it'll work - since I may change it multiple times until it's finished - and I also can't promise it'll ever see the light of day, but I've done some initial experiments and have gotten devices to connect, which is definitely a good sign. I set out to make GBA4iOS the best mobile emulator, if not one of the best overall, and this would be the final piece in the puzzle.

## Wrap-Up ##
Hopefully, this blog post shows that I have in fact been working hard on GBA4iOS, even if I haven't posted as much about it as I would've liked. Making a full-featured emulator is no easy task, especially when you're already having to work around Apple's tight restrictions. I know some of you have begun to get a bit impatient, but you have to understand that I am doing my best to get it released. I'd also like to thank those of you who  realize this and send me supporting tweets and the like, it really means a lot and motivates me to work even harder. I'm doing this all for you, so it really does make it worth it in the end to hear from you guys. So thanks everyone, GBA4iOS 2.0 will be worth the wait!
