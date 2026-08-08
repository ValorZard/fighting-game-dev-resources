# Fighting Game Development Resources
Collection of resources about how to make fighting games of all types, sorted by categories.

Legend:
- ⭐ Key or high quality ressource

## Guidelines for adding new content
1. Add an 1-3 sentence explanation of how this link or resource DIRECTLY relates to fighting games. 
- For example, if you add an article about state machines, you must then explain why state machines are important to fighting games and why reading this article will make you understand their usefulness better.
2. We accept resources for all types of fighting games, including platform fighters and arena fighters. 
- Resources relating to Beat 'em ups like Streets of Rage and Devil May Cry are okay too, since they come from a very similar design lineage.
- Real time action combat in general has a lot of the same design principles and limitations. Both For Honor and Street Fighter use the same basic networking model! (Peer-to-peer deterministic rollback netcode)
3. No Gen AI. We want to have articles and videos made by actual real humans who have made real games, not AI hallucinations that may not actually be true.
4. Try to link to something that has been archived. Stuff like Twitter/X links can get deleted or lost to the mists of time. If you DO want to link to a social media post, make sure it has been backed up somewhere first and link to that backup.

# General

## Engines and Libraries

- [Castagne Engine (Godot, has Rollback)](https://castagneengine.com) - Game engine for fighting and action games focused on efficiency and flexibility. Uses its own custom language and editor.
- [Sakuga Engine (Godot, has Rollback))](https://github.com/NoisyChain/Sakuga-Engine) - Fighting game framework written on top of Godot, using resources to specify movesets. Requires C#/.NET.
- [Night Sky Engine (Unreal, has Rollback)](https://github.com/WistfulHopes/NightSkyEngine) - Fighting game framework written on top of Unreal. Uses blueprints directly instead of a custom scripting layer.
- [IKEMEN (Standalone, has Rollback)](https://ikemen-engine.github.io/) - Open source remake of the famous MUGEN fighting game engine written in Go. Uses its own language and can be extended with LUA. Massive vault of standalone characters made over the years.

## Game Development

- ⭐ [Excellent documentary on Killer Instinct's development](https://youtu.be/ks4eZoG94Vs)
- ⭐ [I Wanna Make a Fighting Game - Tutorial series](https://andrea-jens.medium.com/i-wanna-make-a-fighting-game-a-practical-guide-for-beginners-part-1-2021-update-955a4672eea5)

# Technical / Programming

## Game Inputs
- [Input Buffering, Action Canceling, and also Forbidden Knowledge](https://medium.com/@yosispring/input-buffering-action-canceling-and-also-forbidden-knowledge-47a3f8a95151)

## Networking

- ⭐ [Repository of resources on game networking](https://github.com/0xFA11/MultiplayerNetworkingResources)
- [Visual guide to how rollback network works](https://bymuno.com/post/rollback) - made by someone who worked on Rivals of Aether and Animation Versus
- ⭐ [Rollback Netcode Pseudocode](https://gist.github.com/rcmagic/f8d76bca32b5609e85ab156db38387e9) - THE algorithm on how rollback netcode works
- ⭐ [GekkoNet](https://github.com/HeatXD/GekkoNet) - Modern replacement/spiritual successor to GGPO.
- [Choosing the right network model for your multiplayer game](https://mas-bandwidth.com/choosing-the-right-network-model-for-your-multiplayer-game/) - shows all of the different networking models you can have in your game. Choose the best one for your game!
- [8 Frames in 16ms: Rollback Networking in Mortal Kombat and Injustice 2 - GDC 2018](https://youtu.be/7jb0FOcImdg?si=t1JMQk3E8Efalw2L)

An interesting thread that I found on Twitter thanks to @Rod F https://yal.cc/preparing-your-game-for-deterministic-netcode/ 
https://bymuno.com/post/rollback

# Graphics and Sound

## Art/Animation - General
*Note: While this repository is meant for advice that can help fighting game developers specifically, we thought it would still be nice to offer a curated selection of art resources for those who want to learn how to get started with art in games.*
- ⭐ [12 Principles of Animation (Official Full Series)](https://www.youtube.com/watch?v=uDqjIdI4bF4)

## Art/Animation - Real Time Action Combat
- ⭐ [Making Fluid and Powerful Animations For 'Skullgirls' - GDC 2014](https://www.youtube.com/watch?v=Mw0h9WmBlsw) - Talk by the Lead Animator on the fighting game Skullgirls on how animators are done in that game.

## Graphics Programming - Stylized
- [From mobile to high-end PC: Achieving high quality anime style rendering on Unity](https://youtu.be/egHSE0dpWRw?si=eR1fYJKz4ENuQN8v) - Talk given by miHoYo's lead technical developer on how they achieve the look of Honkai/Genshin Impact
- [From Mobile to Console: Genshin Impact's rendering technology on Console](https://youtu.be/00QugD5u1CU?si=N2TGlAd3AqzScsfr) - Another talk by miHoYo about how they achieved the look of Genshin Impact. (Note: even though the video's title is in Korean, the actual talk is in English.)
- ⭐ [GuiltyGearXrd's Art Style : The X Factor Between 2D and 3D](https://youtu.be/yhGjCzxJV3E?si=IP7BnpiQGauACJtE) - THE talk if you want to understand how Arc System Works achieves the look they've become famous for in their fighting games.
- [Why Guilty Gear 3D Artists Don't Trust the Reference Sheet | Industry Insider Interview](https://youtu.be/vkcnOZ3eVL4?si=rrvXDoN5YBy5mQ6I) - Interview with someone who works in the Japanese video game industry on how to achieve that "3D Anime" look.
- [Panagiotis Tsiapkolis: From watercolors to mechs: Stylized rendering and asset pipelines in Godot](https://www.youtube.com/watch?v=uyGPbbDktnE) - Talk given by the creator of the Castagne Engine, Panthavma.

# Design

## General Game Design

- ⭐ [Infil's Fighting Game Glossary](https://glossary.infil.net/)

Core-A gaming is essentially required reading for anyone trying to make a fighting game https://www.youtube.com/playlist?list=PLWIbhIYLOq-T7XwgHe2y2hBE8Zr_yeODi

Core A Gaming is pretty much essential watching at this point. I also highly recommend Novril Tataki's channel for similar reasons. Several video series, that are meant to teach new players, but are actually great for devs as well. Their older series on Guilty Gear character tutorials also helped me designing movesets. https://www.youtube.com/user/novriltataki

Also add Sugarpunch Design Works. Great for learning about animation basics and sometimes game feel. Not entirely focused on fighting games though. https://youtu.be/s4HKw7Hqqd0

(Sugarpunch definitely has some worthwhile insights, but he also spews out a lot of "hot takes" so take what he says with a grain of salt)

Once I was asked about how I implemented the AI in my game. I might share that info here again. Don't know if it counts as learning material. Feel free to move it/remove it! [Twitter thread] https://twitter.com/AndreaDProjects/status/1086641395740352513?s=20

# Publishers
- [Publisher Contracts: Red Flags](https://ltpf.ramiismail.com/publisher-contracts-red-flags/)
- [Don't Make My Job Easy: Effectively Pitching to Publishers - GDC 2022](https://youtu.be/JZyCgChW0dc?si=Bxs-IfyX0FkvALWL)
# Marketing

# Unsorted
https://www.youtube.com/playlist?list=PLj34EySs1IeZLdaLTIoMvkoMkxUk2l74A

https://www.youtube.com/watch?v=gpXganAM_qA

https://twitter.com/mauvecow/status/1182084533035757568?s=20 a very interesting thread about rollback implementation and what to consider

http://glossary.infil.net/

MarcDWyz🕹 — 2021-06-09 4:17 PM
I did a Q&A about rollback netcode.
➡️  https://youtu.be/AT9gznRM860

https://twitter.com/GxGrainSon/status/1419275528838729736?s=19

https://docs.google.com/document/d/1IeRLLBHUIly9UD5PxXf8sWmaB-lGyTwf/edit

https://www.youtube.com/watch?v=lytuRLkfhus

https://twitter.com/haydndalton/status/1541104969478246403?t=bmIYY5mKLKKTbAu4G90_7g&s=19

http://lindsaycox.co.uk/blog/unity/unity-c-performance-tips-and-tricks/

https://blog.gemserk.com/2017/03/14/using-unity-text-to-show-numbers-without-garbage-generation/

https://learn.jettelly.com/unity-shader-bible/#buy-now

https://answers.unity.com/questions/1359179/does-unity-fixed-foreach-problem-gc-boxing.html

https://www.jacksondunstan.com/articles/3577

https://mobile.twitter.com/YosiSpring/status/1548408537931399178

https://www.youtube.com/playlist?list=PLwXxbJKDwxSUexU-RyPXHYSeq--8pXEON

https://www.schellgames.com/blog/the-definitive-guide-to-playtest-questions

https://rodzilla.itch.io/material-maker

https://www.patreon.com/posts/vfx-breakdown-71191108

https://springrollgames.itch.io/ggmr

https://www.brookaccessory.com/pro.php?m=d&pid=44237976

https://medium.com/kitfox-games/the-indie-game-studio-glossary-6ea8d422065c

http://reports-archive.adm.cs.cmu.edu/anon/2017/CMU-CS-17-128.pdf

https://help.steampowered.com/en/faqs/view/60E5-5E13-712C-5315

https://steamcommunity.com/sharedfiles/filedetails/?id=183672148

https://www.gameuidatabase.com/index.php

https://www.youtube.com/watch?v=J-3avMBqJ9s

https://www.gamesindustry.biz/rami-ismails-top-ten-tips-on-surviving-the-indiepocalypse

https://youtu.be/8wm9ti-gzLM

https://www.youtube.com/watch?v=RzjAVFU4yz8&list=PLKaq87gaP9IEPctr9scliswmcoJ5B7Pnj

https://youtu.be/f4s1h2YETNY

https://www.youtube.com/watch?v=EScvYBJyrdw

https://docs.google.com/presentation/d/1txprTept_SlOCjURlIv-07a_9eDzMiGVT8yZlInOtd8/edit?usp=sharing

https://www.youtube.com/watch?v=E3zHGD8V2IY&t=179s

https://www.reddit.com/r/cpp_questions/comments/152ze93/learning_cpp_as_a_beginner/

https://www.youtube.com/watch?v=XTZVbmz7LpY

https://twitter.com/KenneyNL/status/1690770193327300608

https://www.udemy.com/course/unreal-engine-5-the-ultimate-game-developer-course/

https://www.udemy.com/course/unrealcourse/

https://twitter.com/joewintergreen/status/1701882185375220165

https://www.youtube.com/watch?v=MeMPCSqQ-34

https://www.learncpp.com/

https://twitter.com/panthavma/status/1704235501023019079

https://packetlosstest.com/

https://www.youtube.com/watch?v=-_fP93WDq9w

https://www.reddit.com/r/godot/comments/171rt0q/cursos_y_tutoriales_para_aprender_godot_engine/

https://www.youtube.com/watch?v=2MB9cAwC0Nw

I remember years ago when a single guy inpisred in what the people at Raodmap.sh did, made a roadmap in a similar fashion for Game Dev.
Now, I came back to roadmap.sh and there is a Game Dev roadmap as well. Maybe it is from that guy?
Client side: https://roadmap.sh/game-developer
Server side: https://roadmap.sh/server-side-game-developer

https://www.youtube.com/watch?v=w9W3GpFFIbM

https://twitter.com/SEGA_AM_2/status/1775450937697378310/photo/1

https://www.dataorienteddesign.com/dodbook/

https://github.com/dbartolini/data-oriented-design

https://www.youtube.com/watch?v=rz99vzYY514

https://fxtwitter.com/YosiSpring/status/1823851395402903793

https://feepresskit.com/#/

https://dopresskit.com/

https://happysoulmusic.com

https://www.youtube.com/@GraphicsProgrammingConference

https://medium.com/design-bootcamp/novelty-and-complexity-budgets-fc583e80a055

https://int10h.org/oldschool-pc-fonts/fontlist/

https://www.proko.com/course/figure-drawing-fundamentals

https://drawabox.com/

https://www.youtube.com/watch?v=eRVRioN4GwA

https://youtu.be/9YSqhfjqfgs

https://mathworld.wolfram.com/

https://direct.mit.edu/books/oa-monograph/5572/The-Videogame-Industry-Does-Not-ExistWhy-We-Should

https://www.youtube.com/watch?v=xsZk3c7Oxyw

https://www.youtube.com/watch?v=CU-SZo2dMHk

https://warthogreport.substack.com/p/analyzing-smash-bross-original-design

https://youtu.be/4vdIDygj1bE?si=jipeYE9mfKV52LDy

https://characterdesignreferences.com/

https://www.youtube.com/watch?v=VYW7U98japY

https://www.youtube.com/watch?v=E5M41URxi9k

https://www.youtube.com/watch?v=jz8k8mWYByM

https://www.mixamo.com/

https://github.com/Ensteq/ToonShadingCollection/tree/main

https://www.youtube.com/@takimarueffect_tips

https://lospec.com/ 

https://www.youtube.com/playlist?list=PLnuhp3Xd9PYTt6svyQPyRO_AAuMWGxPzU

https://guide.handmadehero.org/ 

https://www.pcgamer.com/gaming-industry/rpg-developer-owlcat-launches-free-game-dev-learning-resource-a-rising-tide-truly-lifts-all-ships/

https://owlcat.games/learning

https://youtu.be/v1CqFQNNvHc?si=90_fioTa8_kGk0t4

https://ci.itch.io/all-game-assets

https://youtu.be/m4Bwyb52W3E?si=BmK5BzB5VU-wrMvO

https://docs.vulkan.org/tutorial/latest/Building_a_Simple_Engine/introduction.html

https://www.youtube.com/playlist?list=PLImQaTpSAdsArRFFj8bIfqMk2X7Vlf3XF

https://owencmyk.xyz/designing-fighting-games/hold-buffers/

https://github.com/rcmagic/ZigFightingGame/

https://youtube.com/playlist?list=PLcaQc6eQjXCzYski4EEr-iRfdkXkX-P3g

https://animatorsresourcekit.blog/category/assets/reference/

https://setteidreams.net/

https://animatorsresourcekit.blog/2018/02/20/challenger-jacobus/

https://jvns.ca/blog/2023/01/13/examples-of-floating-point-problems/

https://youtu.be/uCPQGncOx-Q

https://coloso.global/en/products/gameartist-remyhobo-us

https://gamedev.tv/courses/blender-sprites

https://www.youtube.com/watch?v=oLu9I7tkfp8

https://docs.google.com/presentation/d/1zP_ns92nUwSJP4fP8abTy2lWopL6h12rZl0AcpEG-jw/edit?usp=sharing

https://youtu.be/TivpMwuGzeM

https://coloso.global/en/products/gameartist-remyhobo-us 

https://www.youtube.com/@moderndayjames/videos

https://itch.io/c/7216862/godot-cheatsheets

https://trueref.io/

https://community.trueref.io/free_references

https://www.youtube.com/watch?v=2F5WBfqf0Sc

https://youtu.be/rRXd_fJowdk 

https://codemanu.itch.io/spritemancer
