---
layout: post
title: "Clicking vs Typing"
description: "Methods of interaction matter"
category: 
tags: []
published: true
author: eli
---
{% include JB/setup %}


As programmers, we live in a world of text. There's a [good reason](http://en.wikipedia.org/wiki/Unix_philosophy) for this. Most of our time programming is spent either in a text editor or at the command line. And because we more or less live inside of these programs, when we make programs, we're usually typing. A lot.

But there's a whole other way of interacting with computers: clicking. It's a method of interaction that many programmers dislike a great deal; many people go to [great lengths](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb?hl=en) to make everything on the computer controllable by typing. 

Before we can think about making programming easier, we should think about what makes programming hard. And the first thing I think of is the volume of raw information you need to have on hand in order to do *anything.*

Clickable interfaces force the program designer to deal with a major constraint - the user can only be presented with so many options. There's only so much real estate, so every available action has to be right there on the screen (or nested in some kind of submenu or something). To me, this highlights something that makes programming hard: *you have to have a whole lot of specialized knowledge before you can do anything useful.* The syntax of the language we're using; the names of variables in the current scope; the contents of the libraries we're including; the commands that we have to issue at the command line. And it gets worse. There are also idioms ("Should I use \_.each or $.each?"), patterns ("How do I implement a singleton in Java again?"), and libraries ("I forget which is faster - lxml or Beautiful Soup…"). And that's not even considering the actual programming concepts at play in the program! There's just *so much fucking stuff to remember*. 

So anything that can be done to cut down on a) the amount of information that you have to [load into your brain](http://www.youtube.com/watch?v=EmEPXXJ4sKw) b) the percentage of that information that you have on hand at any given moment is going to be a thing that's gonna make programming easier. And I think that interfaces that force you to click contain a nugget of widsom.

Here's the thing - where you're clicking on stuff, you don't have to remember a dang thing. It's just right there on the screen in front of you. That's awesome! No thought required. No prior knowledge. Hell - the clickable thing might even have a tooltip that tells you exactly what it does. Maybe it even has a cute icon on it of a penguin or an ice cream cone or whatever. The point is, having something to click on is *fundamentally* different than the blinking cursor of the command line. Sure, you can do way less, but the stuff you can do is way easier. There's a lot of value in **finite, predefined choices**.

So am I saying that you should fork gvim to give it shiny buttons adorned with anime characters? No. I understand why programmers hate clicking; I hate clicking. I get it. It's slow and cumbersome and you have to move your fingers off the precious home row and it's all just dreadfully *inefficient*. So that's not what I'm suggesting.

The thing I think is valuable is simply becoming aware of the fact that remembering stuff is fucking hard, and for some reason, our profession has chosen two tools (the text editor and the command line), that each require the user to remember *insane amounts* of arcane commands and syntaxes and forms and words. If the real benefit of clicking interfaces is **finite, predefined choices**, I'm pretty sure that we can reap the benefits of clicking without having to leave the safety of the keyboard.

Here's my conclusion:

***Building programming tools that put the programmer in the position to choose between a set of finite, predefined choices as often as possible will make programming way, way easier.***

But what do you think? Am I off base? Is it impossible?


