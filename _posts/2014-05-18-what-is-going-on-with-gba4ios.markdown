---
layout: post
title: "What is Going On with GBA4iOS?"
date: 2014-05-18 17:10:36 -0500
comments: false
category: blog
author: riley
tag:
- gba4ios
- developer
- nintendo
---

Many of you have shared your concerns over the future of GBA4iOS in regards to some events that have happened in the past week. While [my partner Paul Thorsen](http://twitter.com/pau1thor) and I have been hard at work responding to these issues, we have failed to communicate exactly what was going on, and what steps we were taking to bring GBA4iOS back from its untimely DMCA death. As such, I've written this blog post in an effort to fill everyone in on why GBA4iOS was taken down, what Paul and I are doing to put GBA4iOS back up for download again, and also to correct some misinformation intentionally being spread in order to tarnish the reputation of GBA4iOS, Paul, and myself. Hopefully, by the time you are done reading this, any questions you may have about GBA4iOS' future will be answered, and you may resume happily playing your favorite Game Boy games.

<!-- more -->

Last Tuesday, May 13th, I received the following email from GitHub:

> We received a DMCA takedown notice regarding your GitHub Pages site www.gba4iosapp.com
> As such, we have disabled the page.
> You can view the notice at https://github.com/github/dmca/blob/master/2014-05-13-Nintendo.md  
> 
> If you do not believe you are violating these copyrights you can file counter-notice to have the repos reinstated.
> You can find details on the counter-notice procedure here: https://help.github.com/dmca
> If we do not receive counter-notice within 14 days, the repo cannot be reinstated.

Apparently, Nintendo had issued a DMCA takedown notice to GitHub (my website host) requesting that access to [GBA4iOSApp.com](http://gba4iosapp.com) be disabled. While reading through the DMCA notice (the entirety of which can be found [here](https://github.com/github/dmca/blob/master/2014-05-13-Nintendo.md)), one  particular section stood out, which I've reproduced below (emphasis mine):

> This web site hosts a downloadable mobile application for iOS that **provides users with access to unauthorized and illegal copies of Nintendo’s copyright-protected video games** in violation of Nintendo’s exclusive rights.

Many of you had guessed that the reason Nintendo issued the DMCA takedown request was because GBA4iOS pointed directly to a ROM downloading site, and after carefully reading the DMCA notice it appears this is the case. Nowhere in the notice does Nintendo cite the app's ability to play ROMs, which makes sense, considering emulation itself is perfectly legal in the United States.

With this information, we've decided to no longer point users to any particular ROM downloading site in a future 2.0.4 update. Instead, the web browser will take users directly to Google, allowing them to use the in-app web browser for a multitude of other reasons, such as looking up game tutorials. We debated the best course of action to follow, and eventually decided this would be best for our users, and also would allow us to bring GBA4iOS back as soon as possible. GBA4iOS' primary focus has always been to give everyone the best emulation experience on iOS, and not to promote piracy; hopefully with the removal of the direct links to a ROM downloading site this focus will become more clear.

When can you expect GBA4iOS to be available for download again? I'd expect it to be available in the next few days. In addition to the modification of the in-app web browser, Paul and I have been removing other copyright infringing aspects of the app—such as the use of the Game Boy Advance logo in some controller skins—but we should be finishing that up shortly. However, along with the website, the [GBA4iOS GitHub repo](http://github.com/rileytestut/gba4ios/) was also shut down. I'll do my best to bring it back up once we've updated the app, but no promises; I may need to find another host for GBA4iOS' code.

So, an update to GBA4iOS will be out shortly, and with this update the website and download links will be up again for everyone. I know this entire incident has been inconvenient for everyone involved, and it is entirely our fault; we never should have linked directly to a ROM downloading site in the first place, and Nintendo was only protecting their IP. So please, don't boycott Nintendo because of this; they are an incredible company who produces some of the highest quality video games in the world. If it wasn't for them, GBA4iOS wouldn't exist in the first place.  

<br/>

## One Problem Solved, Another Just Beginning

Unfortunately, some people have taken advantage of this legal incident in order to spread misinformation regarding myself and GBA4iOS, without performing their own research to ensure their facts were true. Following the takedown of GBA4iOS, I came across this tweet:

<blockquote class="twitter-tweet" data-cards="hidden" lang="en"><p>Here is the extent of 18-year old kid rileytestu&#39;s &#39;rebranding&#39; of VBA-M - a &#39;Coolroms partnership&#39; tickback - <a href="https://t.co/BLO7Jcj26g">https://t.co/BLO7Jcj26g</a></p>&mdash; libretro (@libretro) <a href="https://twitter.com/libretro/statuses/466835299956711424">May 15, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

While you might not have heard of @libretro, there's a good chance you know their work: they developed the Libretro API, which is used to play multiple emulators on RetroArch, and many of Libretro's modified emulator cores are used to power [the incredible OpenEmu emulator for Mac](http://openemu.org). I have a huge amount of respect for all that they have done, which is why I was so surprised to see this tweet. Not only were they asserting that I simply rebranded VBA-M and claimed it as my own (which is especially surprising, because RetroArch also uses VBA-M as an emulator core), but also that I had formed a monetary partnership with CoolROM in an effort to capitalize on GBA4iOS' success. Trying to clear up any confusion, I replied with this tweet:

<blockquote class="twitter-tweet" data-conversation="none" lang="en"><p><a href="https://twitter.com/libretro">@libretro</a> I think there&#39;s a misunderstanding here. CoolROM hosts the IPA, and in return I point users to their site. No monetary transaction</p>&mdash; Riley Testut (@rileytestut) <a href="https://twitter.com/rileytestut/statuses/466840953974583296">May 15, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

They did not respond.

Thinking it was still a simple misunderstanding, I decided to ignore the entire incident. However, I soon found out that @libretro was continuing to spread falsified information about my partnership with CoolROM, and people were starting to believe it. As another attempt to clear things up, I offered to share the entire details behind my partnership with CoolROM:

<blockquote class="twitter-tweet" data-conversation="none" lang="en"><p><a href="https://twitter.com/libretro">@libretro</a> <a href="https://twitter.com/nintyapple">@nintyapple</a> partnership link is purely for analytics. I&#39;d be happy to supply you with all communication between CoolROM and I</p>&mdash; Riley Testut (@rileytestut) <a href="https://twitter.com/rileytestut/statuses/467037123770449921">May 15, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet" data-conversation="none" lang="en"><p><a href="https://twitter.com/rileytestut">@rileytestut</a> <a href="https://twitter.com/nintyapple">@nintyapple</a> Please do - it would make you look better than you&#39;re looking right now.</p>&mdash; libretro (@libretro) <a href="https://twitter.com/libretro/statuses/467037449332723712">May 15, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet" data-conversation="none" lang="en"><p><a href="https://twitter.com/libretro">@libretro</a> How would you like the information? Screenshots? Forwarded emails? Don&#39;t want to be accused of falsifying documents</p>&mdash; Riley Testut (@rileytestut) <a href="https://twitter.com/rileytestut/statuses/467037863138193408">May 15, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet" lang="en"><p><a href="https://twitter.com/rileytestut">@rileytestut</a> <a href="https://twitter.com/cl0bber">@cl0bber</a> suggests you put it on your Twitter for all to see. I tend to agree with that approach.</p>&mdash; libretro (@libretro) <a href="https://twitter.com/libretro/statuses/467038758463094784">May 15, 2014</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

Because they never actually specified how they would like the information to be presented, I've opted to reproduce the emails in text on Pastebin, which you can view [here](http://pastebin.com/mY11qZ7D). They've been copied in their entirety, and only slightly modified in order to hide sensitive information (such as the changing of names, or redacting server credentials).

Hopefully, this clears up any confusion regarding the partnership between CoolROM and GBA4iOS. GBA4iOS was not developed to earn money; it is and always will be completely free. As of now, I haven't heard a response back from Libretro, but if I do I will post it here immediately. As stated before, I respect all the work Libretro has done to better the emulation community, and hope this entire issue can be put to rest; we're both working towards making the best emulation experience for our users after all.

Who knew developing an iOS app lying in a legal gray area and distributed outside of the App Store could be so difficult?
