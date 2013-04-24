---
layout: post
title: "Clicking vs Typing"
description: "Methods of interaction matter"
category: 
tags: []
published: true
discoverable: true
author: eli
publish_date: 2013-04-24 00:00:00
---
{% include JB/setup %}

In my [previous post](http://www.thoughtmachine.co/what-makes-programming-hard-pt-1), I talked about how one of the things that makes programming hard is that we need to keep a lot of *stuff* in our brains while we program, no matter how experienced we are. In light of this problem, I think it's useful to examine the ways in which we interact with the computer while we're programming, since there's a lot of opportunity for interfaces to make this problem better.

As programmers, we live in a world of text. There's a [good reason](http://en.wikipedia.org/wiki/Unix_philosophy) for this. Most of our time programming is spent either in a text editor or at the command line. And because we more or less live inside of these programs, when we make programs, we're usually typing. A lot.

But there's a whole other way of interacting with computers: clicking. It's a method of interaction that many programmers dislike a great deal; many people go to [great lengths](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb?hl=en) to make everything on the computer controllable by typing. However, clicking offers an interesting counterpoint to typing.

Clickable interfaces introduce a major, positive constraint - the user can only be presented with so many options. There's only so much real estate on the screen, so every available action has to be right there in front of you (or nested in some kind of submenu or something). And that constraint really helps with the "remembering stuff" problem.

Here's the thing - where you're clicking on stuff, you (ideally) don't have to remember *anything*. It's just right there on the screen in front of you. That's awesome! No thought required. No prior knowledge. Hell - the clickable thing might even have a tooltip that tells you exactly what it does. Having something to click on is *fundamentally* different than the blinking cursor of the command line. Sure, you can do way less, but the stuff you can do is way easier to find. There's a lot of value in **finite, predefined choices**.

So am I saying that you should fork gvim to give it shiny buttons adorned with anime characters? No. I understand why programmers hate clicking; I hate clicking. I get it. It's slow and cumbersome and you have to move your fingers off the precious home row and it's all just dreadfully *inefficient*. So that's not what I'm suggesting.

The thing I think is valuable is simply becoming aware of the fact that remembering stuff is really hard, and for some reason, our profession has chosen two tools (the text editor and the command line) that each require the user to remember *an insane amount* of arcane commands and syntaxes and forms and words. If the real benefit of clicking interfaces is **finite, predefined choices**, I'm pretty sure that we can reap the benefits of clicking without having to leave the safety of the keyboard. Most autocomplete and tab-completion systems are successful because they allow the user to remember less and type less, while retaining the freedom and efficiency of the keyboard.

In summary:

###Building programming tools that put the programmer in a position to choose between a set of finite, predefined choices as often as possible would make programming way, way easier.

