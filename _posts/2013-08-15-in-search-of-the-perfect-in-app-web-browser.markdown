---
layout: post
title: "In Search of the Perfect In-App Web Browser"
date: 2013-08-15 11:05
comments: true
categories:  
- developer
- open source
- GBA4iOS
- RSTWebViewController
---

(Warning, technical developer jargon up ahead).

Before GBA4iOS became well known, it included an in-app web browser to download ROMs. It was a nice feature to have, but the code that actually handled the downloading was rather hacky and didn't work sometimes for apparently no reason. In addition to this, it lacked many features such as a progress indicator and the ability to go forwards and backwards through the browsing history. As such, for version 1.6.1 (the current version), I ditched the web browser all together, opting instead to launch Safari and let the download happen there. However, I knew this was a temporary solution, and I planned to bring back the in-app browser as soon as I could make it awesome.

Spoiler alert: in 2.0, the browser's back, baby.

<!-- more -->

I started by searching around for a good, open-source component that I could drop in with little or no modifications. Despite having quite a few to choose from, I just couldn't find one that fit my needs. That's not to say the ones already out there are bad, [SVWebViewController by Sam Vermette](https://github.com/samvermette/SVWebViewController) is an excellent component and I was strongly considering it for GBA4iOS. However - and understandably so - all current implementations of UIWebViewControllers felt very iOS 6-ish, and each would require a fair bit of modification to reflect the new iOS 7 design. Plus, practically no web view controllers supported downloading, so I'd have to write all that code for myself anyway. With all this in mind, I decided it would actually be *less* work to just write my own.

So that's what I did. Introducing RSTWebViewController:

{% img center ../../../../../images/posts/RSTWebViewController_Preview.PNG RSTWebViewController %}

The design was heavily inspired by iOS 7 Mobile Safari, as you can clearly see. Of course, because it uses standard UIKit controls, you can change the tint color as you see fit (it's currently using GBA4iOS's purple theme).

As for its feature set, I'm aiming to keep this as lightweight as possible. However, three notable features I've added are a progress indicator (which is the purple bar you see in the navigation bar), the ability to share links via custom UIActivities (as opposed to static UIActionSheets most other components use), and an optional delegate method that's called when the entire page is done loading, as opposed to just a single frame.

More importantly though, it has built-in support for downloading files via its downloadDelegate property. Thanks to some new iOS 7 APIs, this was very simple to do, and it's also very easy for you to intercept the download and handle everything yourself if you choose to. 

Here's the RSTWebViewControllerDownloadDelegate protocol declaration as of this writing (redact-ified due to iOS 7 NDA):

{% gist 6245198 %}  

I'm working on RSTWebViewController in conjunction with GBA4iOS (the two go hand in hand after all), so it's still a work in progress. Once I release 2.0, I'll push this code to Github shortly after, and I'll write up a typical release post with all the features and how to use it. In the meantime, I'd love to know your thoughts on yet another UIWebViewController, especially if you have any ideas on what could be included (I'm aiming to keep it nice and simple, but if there's a glaring feature most web browsers don't have I'd be interested in knowing about it so I can decide for myself). 

You can reach me at [my email](mailto:riley@rileytestut.com), [@rileytestut on Twitter](http://twitter.com/rileytestut), or in the comments below.
