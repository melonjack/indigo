---
layout: post
title: Delta Features - Inputs
date: 2017-09-13
comments: true
category: blog
author: riley
tag:
- developer
- delta
- delta features
---

When playing games in Delta, there will be three primary ways to control the games:

* Touch screen
* MFi Controllers
* Hardware Keyboards

I’ll break down these three input methods below:

## Touch Screen

Just like with GBA4iOS, Delta will support customizable controller skins, which will handle touches and convert them to game inputs. By default, Delta will include standard controller skins for each supported game system that mimic the look and feel of that system's controls, such as this controller skin for SNES games: 

![SNES ControllerSkin](/assets/images/posts/delta/snes_controller_skin.png)

However, you are not limited to these standard controller skins. Additional controller skins can be easily created by others and downloaded from Safari, allowing anyone to design and share their own controller skins with the world. More information about the Delta controller skin format will come closer to Delta's release.

## MFi Controllers

While controller skins serve as a beautiful way to play games, some games require more complex control schemes that cannot be easily performed on a touch screen. Apple realized this too, and with iOS 7 brought official support for MFi-certified game controllers. Of course, Delta supports all MFi controllers, allowing you to use real physical buttons when playing games.

However, the buttons on MFi controllers don't exactly match up with any of Delta's emulated systems. For instance, GBC games have A, B, Start and Select buttons, whereas MFi controllers have A, B, X, Y buttons, but no Start and Select. To compensate for this, Delta will have a default input mapping for each system that we felt was as convenient as possible (such as in this case, mapping the MFi controllers X and Y buttons to GBC's Select and Start inputs, respectively). 

Of course, these default input mappings may not work well for you or the games you're playing, so you are able to create your own input mappings to change _any_ controller input to the game input of your choice. Additionally, you'll even be able to map controller inputs to certain Delta features such as Fast Forwarding or Save States for even more convenience!

![Input Mapping](/assets/images/posts/delta/input_mapping.png)

## External Keyboard

Finally, Delta also supports using external keyboards as game controllers, which includes both bluetooth keyboards and those connected via iPad Pro’s Smart Connector. Naturally, this is especially convenient for iPads with a connected Smart Keyboard, since the keyboard is always with you!

Just like with MFi Controllers, Delta will define a default mapping of keyboard keys to game inputs for each system, which of course will also be able to be fully customized, including mapping keys to Delta-specific features as well.

## Conclusion

Delta will ship with these three forms of input, however we hope to add additional forms in the future, such as using other nearby iOS devices. Until then, these input methods should be more than sufficient for practically any type of game imaginable, and we can’t wait for you to try them out!

Also, keep your eyes peeled for the next Delta Features post, where we’ll dive into some new iPad-exclusive features 😉.
