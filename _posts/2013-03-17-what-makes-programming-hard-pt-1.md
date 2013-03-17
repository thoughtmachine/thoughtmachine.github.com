---
layout: post
title: "What Makes Programming Hard? Part 1"
description: "Knowing is half the battle."
category: 
tags: []
published: true
author: eli
---
{% include JB/setup %}

<div class="explanation">
Before talking about how to make programming easier, we should probably talk about why programming is hard to begin with.
</div>

A couple of years ago, I decided that it would be cool to try and teach some of my non-engineer coworkers how to program. I set up a small course, and bunch of people signed up. I was pumped.

If the course was going to be exciting for people who were learning how to program, we would have to make something tangible and useful. Like a website! Perfect. We would all think of simple webapps that we wanted to make, and then we'd make 'em.

So I made a syllabus for the whole thing, and it seemed pretty realistic. We would spend a day on HTML, a day on CSS, then a few days on PHP basics. Maybe we would even get to SQL! As someone who's been programming for a little while, the concepts seemed pretty simple, especially if they were explained well (and naturally, I was pretty confident that I would explain them well). HTML is just tags! CSS is just selectors and rules! Easy. 

You probably can see how foolish it was of me to think that I could cram all that info into an 8-week course. And yeah, the curriculum was ambitious. But the things is - you *need* all of that information if you want to build a functional website. Even if we were going to be using a framework that offered a very high level of abstraction (like Ruby on Rails, for example), we would *still* need to master at least three completely different languages in order to do anything interesting.

What's worse is that using something like Ruby on Rails introduces a *whole different set* of concepts that need to be understood (models! migrations! partials! asset pipeline!). 

A lot of people advocate the "blind mimicry" school of teaching people to program - just doing what the instructions prescribe, without describing the meaning of the syntax, or the totality of the concepts involved. Which I guess circumvents the practical implications of this problem, but the problem still stands:

***To make any sort of computer program, even a very simple one, the amount of trivia you need to know is completely bananas.***

And I'm not talking about the stuff you need to *understand*. Just the stuff you need to *know*. I still don't understand much of what the computer is doing at any given moment (when I'm programming, or otherwise). For example, I still don't fully *understand* the Unix permission model. However, I do *know* how to overcome most permission problems - I've picked up enough tricks with chown and chmod to get around most common hiccups.

So even if you understand, conceptually, what CSS is, you have to just know *so much stuff*. What's the rule for making text italicized? How about centering an image in the exact middle of the page? Turning all the links green?

This isn't just a problem that affects noobs, either. Paradoxically, the better you get at programming, the more stuff you need to know at any given moment. I think this has some sort of connection to the [efficiency paradox](http://en.wikipedia.org/wiki/Jevons_paradox), but I'm not totally sure what it is. If you're someone who programs a lot, you don't have to think twice about how to iterate through a list in Python. It's in muscle memory, and pulling it up doesn't consume any brainpower. However, you're now aware of a multitude of other data points, all of which need to be available for recall at a moment's notice - the naming conventions for the project you're working on, the fact that method foo is really computationally expensive and shouldn't be called very often, the order of the parameters to the Bar constructor, and so on. 

Googling helps. And Stackoverflowing. Hell, those two sites have been integral to my ability to program *anything*. At the very least, they make this problem a bit less painful. However, they're not a panacea: for beginners, you have to know a certain amount to even search for answers effectively (it's sort of like how you need to know the fundamentals of spelling before you can look up a word in the dictionary). And for experts, no site on earth is going to help you manage the huge amount of information that you need to have in hand to deal with *your* project.

As humans, our short-term memory has a [pretty low ceiling](http://en.wikipedia.org/wiki/The_Magical_Number_Seven,_Plus_or_Minus_Two). And programming **blows this limit out of the water**.

If programming were writing in English prose, this problem would be the equivalent of having to learn new vocabulary words for each document that you wrote. Some of them would have very similar meanings to other words that you knew, but would be spelled totally differently. Others would be spelled similarly, but have dramatically different meanings. Others would have the *exact same spellings*, but different meanings depending on the context. And there would be *thousands* of these words. And if this is a professional project, you're working on this document with hundreds of other people, each of whom are modifying the dictionary at will. And the definitions for each of these words are spread across thousands of different text files. And if you misuse a word, *things explode*.

A lot of the pain of having to *know* is offset by our ability to *understand*. For example, if you can build up a mental model of how you've organized all the objects in your system, you don't have to store all of their names in your short-term memory; you can simply query the mental model you've got built up. But here's the thing - understanding in programming is almost as difficult as knowing. And this will probably the topic of part 2. 

- it doesn't get easier - the cliff remains constant
- compare to written english
- you don't need to know everything if you understand a lot - but understanding is fractal