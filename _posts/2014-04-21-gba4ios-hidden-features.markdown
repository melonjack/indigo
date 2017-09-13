---
layout: post
title: "GBA4iOS Hidden Features"
date: 2014-04-21 19:59:07 -0500
comments: true
category: blog
author: riley
tag:
- developer
- gba4ios
---

Twenty-five years ago today, the Game Boy was born. With it came a wide array of exciting new games—including the first of many incredible Pokemon games—and the ability to play them wherever you were, because the system was small enough to fit in your pocket. Sadly, I never owned the original Game Boy, but one day my parents gave my siblings and me its successor: the Game Boy Color. I fell in love with it the moment I got it, and carried it around with me everywhere (and of course, we got the light accessory to shine on the screen, because this was before Nintendo added backlighting). 

Now, twenty-five years later, the gaming landscape has changed dramatically. Not only has Nintendo's own products evolved to essentially science-fiction levels of sophistication by 1989 standards (glasses-free 3D anyone?), but other companies have found themselves achieving tremendous success in the video game market, even those who originally had no intention of competing. Of course, I'm referring to Apple and the release of iPhone (and subsequently the App Store). I'm sure no one predicted that a mobile phone could disrupt the portable video game market as much as it did, but today it's becoming more and more difficult to develop a game for dedicated game consoles when people are choosing to pay only a couple of bucks for a game on a device they already have with them at all times. 

However, these classic Nintendo games still hold a place in many of our hearts, if only for the nostalgia we get from playing them and the countless hours spent trying to perfect our skills. It was because of this that I set out to develop the best Game Boy emulator for iOS, and with the release of GBA4iOS 2.0 just over two months ago, I'm closer than ever to achieving that goal. Of course, I still plan on updating the app with new features—expect linking between devices and the ability to change the color of original Game Boy games in a future update—but 2.0 is already home to a large number of features; some more obvious than others. 

These less obvious features are why I decided to write this blog post; GBA4iOS is home to many features that people don't know about, so I thought it would be best for them all to be collected in one place. More than likely you'll know a few of these already, but I expect that most of you will discover a feature you didn't already know about! Either way, it can't hurt to relearn a feature you may have forgotten, so hopefully all of you will get something out of this post. If not, well, you always have future updates to look forward to!

So, without further adieu, here are all the obscure features of GBA4iOS.

<!-- more -->

## Share Games
Many of you have requested the ability to sync games between devices. For sake of simplicity and to not fill up valuable Dropbox space on games that can be redownloaded, I've opted not to do this. However, if you press and hold on a game in the main menu, you can then choose to share the game via email, or by AirDrop if your device supports it.

![Share Game](/assets/images/posts/hidden_features/share_game.png)  

<br/>

## Rename Games
Similarly to sharing games, if you press and hold on a game in the main menu, you can select the option to rename the game to whatever you want. Even better, renaming will not mess up syncing, saving, or anything else tied to a game; it just works!

![Rename Game](/assets/images/posts/hidden_features/rename_game.png)  

<br/>

## Protect and Rename Save States
Save states are a valuable part of any emulator, so I wanted to make sure they were powerful. In GBA4iOS 2.0, pressing and holding on any save state will give you the option to rename it or protect it. Renaming does exactly what you'd think: you can name it anything you want for easier identification later. Protecting is something unique to GBA4iOS: once you protect a save state, you can no longer overwrite it. This is great for save states you want to keep when something exciting happens in a game, and you don't want to ever accidentally overwrite it. Of course, you can always unprotect a save state later.

![Protected Save State](/assets/images/posts/hidden_features/protect_save_state.png)  

<br/> 

## Download Games From Other Websites
By default, the in-app game downloader takes you to [CoolROM.com](http://coolrom.com) to help you download games easier and faster. However, if you'd prefer to download from somewhere else, no problem!  Just tap the back button in the web browser, and it will take you to a Google search page where you can search for whatever game-downloading website you'd like and download games fom there.

Bonus hint: you can also download games from Safari on your device, and then tap "Open In" and select GBA4iOS to import them into the app.

![Share Game](/assets/images/posts/hidden_features/google_search.png)  

<br/>

## URL Scheme Support
On iOS, apps can declare custom URL schemes, which allows others apps to open up the app. GBA4iOS makes use of this, and you can see this for yourself by typing "gba4ios://" into Safari and watching as it launches GBA4iOS. This technique also allows you to open particular games automatically from apps such as Launch Center Pro or from the Home Screen directly via Web Clips, assuming you configure the URL correctly. GBA4iOS' URL schemes are extremely powerful, and I'd recommend checking out [Dario Sepulveda's in-depth tutorial on how to make your own GBA4iOS shortcuts](http://gba4ios.mithical.com/post/79900431497/gba4ios-2-0-url-schemes-part-1-introduction).

![Launch Center](/assets/images/posts/hidden_features/launch_center.png)  

<br/>

## Event Distribution
Another GBA4iOS-exclusive, this feature allows you to download special events for Game Boy Advance Pokemon games, where you can receive special items or Pokemon from yours truly! So far, there have been two events, but I have many more planned ranging from receiving some rare items to catching the elusive Mew. To check for events, start the Pokemon game of your choice, tap the Menu button, then tap "Event Distribution". Here, you can view all the events you've downloaded or that are available to download, and this menu is also where you can start the events for your game.

![Event Distribution](/assets/images/posts/hidden_features/event_distribution.png)  

<br/>

## Wario Ware: Twisted! Support
One of my favorite Game Boy Advance games of all time is Wario Ware: Twisted!, and while the original Wario Ware was playable on GBA4iOS, Twisted! required use of an external gyroscope adaptor, which there was no support for. However, in 2.0 this gyroscope has been specifically emulated in order to allow everyone to experience Wario Ware: Twisted! as if it was on an actual Game Boy Advance. If you haven't yet, I'd definitely recommend giving it a try.

![Wario Ware: Twisted!](/assets/images/posts/hidden_features/wario_ware_twisted.png)  

<br/>

## Sustain Button
As convenient as it is to be able to play all your Game Boy games wherever you are, sometimes touch screen buttons make the games much harder to play. Because of this, GBA4iOS added support for official MFi iOS 7 Game controllers, but I also knew that not everyone had access to one of these controllers. Because of this, Sustain Button was born. When playing a game, tap the Menu button, then tap "Sustain Button". Now, you can select the button you want GBA4iOS to hold down for you, such as the "run" button in Pokemon or the "accelerator" in Mario Kart. This frees up your fingers to press other buttons instead, which can be the difference between winning and losing a game. To unsustain a button, simply enter the Sustain Button selection screen again and tap anywhere there isn't a button.

![Sustain Button](/assets/images/posts/hidden_features/sustain_button.png)  

<br/>

## Hidden Skin Features
The primary function of controller skins is to change the look of the controller being used in game. However, skins have a lot more power than just changing the image; they also have the ability to change the mappings of buttons to be bigger or smaller, add or remove certain buttons, or even change the location of the screen. In fact, GBA4iOS 2.0.2 adds the ability to resize the screen however you want, allowing for true full screen landscape modes, or any other crazy design skin designers come up with. You can download custom skins in-app from the skin settings in GBA4iOS, or from a 3rd-party skin site such as [GBA4iOSkins.com](http://www.gba4ioskins.com).

![Controller Skin Features](/assets/images/posts/hidden_features/controller_skin_features.png)  

<br/>

## And Finally...Draggable External Controller Buttons
Okay, so this isn't really a feature, but more of a more fun way to accomplish a task. With support for MFi iOS 7 Game Controllers comes the ability to customize what each button on the controller does in GBA4iOS. To customize this, normally you'd go to Settings \> Configure Buttons, and tap each button to change what action it does. However, most of the time you simply want to switch the function of two buttons, and you can accomplish this by dragging the black pop-up above each button to a new button. Even if you don't have an iOS 7 controller, it's fun to play with!

![Configure Buttons](/assets/images/posts/hidden_features/configure_buttons.png)  

<br/>

After going through the app carefully, that's all the features I could find that I thought were somewhat obscure, but worth knowing about. Of course, even though I made the app it's entirely possible I forgot about some features. If you've discovered a feature I left out, feel free to put it in the comments; it's always great to see what others have discovered. Hopefully though, I listed enough for you all to discover one thing about the app you didn't already know, so go and have fun with whatever feature it may be!
