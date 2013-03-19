---
layout: post
title: "What Makes Programming Hard? Part 1"
description: "Knowing is half the battle."
category: 
tags: []
published: true
discoverable: false
author: eli
---
{% include JB/setup %}

Before talking about how to make programming easier, we should probably talk about why programming is hard to begin with. I've come up with a couple of problems, and I'll try to do a post on each one.

##Problem #1: Knowing Stuff

A couple of years ago, I decided that it would be cool to try and teach some of my non-engineer coworkers how to program. I set up a small course, and a bunch of people signed up. I wanted to make the course interesting and relevant for them, so I decided that we would all make dynamic websites.

I made a syllabus for the whole thing, and it seemed pretty realistic. We would spend a day on HTML, a day on CSS, a few days on PHP basics, and a day on SQL. As someone who's been programming for awhile, the concepts seemed pretty simple, especially if they were explained well (and naturally, I was pretty confident that I would explain them well). HTML is just tags! CSS is just selectors and rules! Easy. 

What's amazing is, at first, it actually *was* kind of easy. People started to get it. HTML *is* just tags! Cool! Everything seemed like it might actually work out.

The problem arose when CSS was introduced. People understood what it was for, and how it related to HTML. But learning a completely new  *syntax* and *vocabulary* really slowed them down.

The thing that I noticed most, watching my students struggle to make their webpages look the way they wanted them to look, is just how much *arbitrary information* they needed to ingest. They needed to know that a link is, counterintuitively, represented by the <span class="mono">a</span> tag and not the <span class="mono">link</span> tag. They needed to remember that every CSS rule needs to end in a semicolon, or things fail silently. They needed to know about <span class="mono">float</span> and <span class="mono">clear</span> and the fact that <span class="mono">div</span> defaults to <span class="mono">display: block</span> but <span class="mono">span</span> doesn't. *And they were still dealing with the easy stuff.*

So I think the first difficulty of programming could be summarized thusly:

***To make any sort of computer program, even a very simple one, the amount of arbitrary stuff you need to know is completely bananas.***

-------

Google helps. And Stack Overflow. However, they're not a panacea: for beginners, you have to know a certain amount to even search for answers effectively (it's sort of like how you need to know the fundamentals of spelling before you can look up a word in the dictionary). And for experts, no site on earth is going to help you manage the huge amount of information that you need to have on hand in order to deal with *your* project.

For this reason, getting better at programming doesn't make this problem go away. So if you're someone who programs a lot, you don't have to think twice about how to, say, iterate through a list in Python. It's in muscle memory, and pulling that factoid up doesn't consume much brainpower. However, you're forced to become aware of a multitude of *other* data points, all of which need to be available for recall at a moment's notice: the naming conventions for the project you're working on; the fact that method <span class="mono">foo</span> is really computationally expensive and shouldn't be called very often; the order of the parameters to the <span class="mono">Bar</span> constructor; and so on. 

OK, so, yeah, the amount of stuff you have to know in order to program is pretty big, and it doesn't get smaller as you get better. However! A lot of the pain of having to *know* is offset by our ability to *understand*. For example, if you can build up a mental model of how you've organized all the Javascript files in your project, you don't have to store all of their names and locations in your short-term memory; you can simply query the mental model you've got built up. 

But here's the thing - understanding in programming is almost as difficult as knowing. And this will be the topic of part 2. 