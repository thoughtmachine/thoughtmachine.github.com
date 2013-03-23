---
layout: post
title: "What Makes Programming Hard? Part 1"
description: "Knowing is half the battle."
category: 
tags: []
published: true
discoverable: true
author: eli
---
{% include JB/setup %}

Before talking about how to make programming easier, we should probably talk about why programming is hard to begin with. I've come up with a couple of problems, and I'll try to do a post on each one.

###Problem #1: To make any sort of computer program, the amount of arbitrary stuff you need to know is completely bananas.

A couple of years ago, I decided that it would be cool to try and teach some of my non-engineer coworkers how to program. I set up a small course, and a bunch of people signed up. I wanted to make the course interesting and relevant for them, so I decided that we would all make dynamic websites.

I made a syllabus for the whole thing, and it seemed pretty realistic. We would spend a day on HTML, a day on CSS, a few days on PHP basics, and a day on SQL. As someone who's been programming for awhile, the concepts seemed pretty simple, especially if they were explained well (and naturally, I was pretty confident that I would explain them well). HTML is just tags! CSS is just selectors and rules! Easy. 

What's amazing is, at first, it actually *was* kind of easy. People started to get it. HTML *is* just tags! Cool! Everything seemed like it might actually work out.

The problem arose when CSS was introduced. People understood what it was for, and how it related to HTML. But learning a completely new  *syntax* and *vocabulary* really slowed them down.

The thing that I noticed most, watching my students struggle to make their webpages look the way they wanted them to look, is just how much *arbitrary information* they needed to ingest. They needed to know that a link is, counterintuitively, represented by the <span class="mono">a</span> tag and not the <span class="mono">link</span> tag. They needed to remember that every CSS rule needs to end in a semicolon, or things fail silently. They needed to know about <span class="mono">float</span> and <span class="mono">clear</span> and the fact that <span class="mono">div</span> defaults to <span class="mono">display: block</span> but <span class="mono">span</span> doesn't. *And they were still dealing with the easy stuff.*

Something really struck me as I watched them: Even though I've been programming for years, I still have the same problem - I need to keep an unmanageable amount of arbitrary stuff in brain.

Certain aspects of this problem definitely do get easier with experience. For example, I don't have to think twice about how to, say, iterate through a list in Python. It's in muscle memory, and pulling that factoid up doesn't consume much brainpower. I've also figured out how to use Google and Stack Overflow to get answers to most common problems (which is actually tough for a beginner to do - they have to know enough to know how to formulate the question). However, no site on earth is going to help me manage the huge amount of information that I need to have on hand in order to deal with *my particular* project.

So even though I can call up the syntax and vocabulary for a given language pretty easily, I'm forced to become aware of a multitude of *other* data points, all of which need to be available for recall at a moment's notice: the fact that method <span class="mono">foo()</span> is really computationally expensive and shouldn't be called very often; the order of the parameters to the <span class="mono">Bar</span> constructor; what the hell I named the thing that fetches the data from the <span class="mono">/quux</span> endpoint; and so on. 

There are a bunch of fields that require their practitioners to know a huge amount of arbitrary information: medicine and law come to mind. The difference with programming, and the real root of the problem, is that we have the luxury of being able to query vast storehouses of knowledge while on the job, *but for some reason this doesn't make things easier*. A lawyer can't consult a statute while arguing a point; a surgeon can't break out their smartphone in the middle of an operation. But we have the good fortune to be seated in front of an amazing information-retrieval device while we do our work. The fact that we're in this privileged situation, yet we're still required to memorize tons of arbitrary information, is a failure of our ability to utilize the computer to the fullest extent of its capabilities.

We can design programming environments to make this problem less painful. Why haven't we?