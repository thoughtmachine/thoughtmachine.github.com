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

So I made a syllabus for the whole thing, and it seemed pretty realistic. We would spend a day on HTML, a day on CSS, then a few days on PHP basics. As someone who's been programming for a little while, the concepts seemed pretty simple, especially if they were explained well (and naturally, I was pretty confident that I would explain them well). HTML is just tags! CSS is just selectors and rules! Easy. 

What's amazing is, at first, it actually *was* kind of easy. People started to get it. HTML *is* just tags! Cool! Everything seemed like it might actually work out.

The problem arose when CSS was introduced:

1. There was now a second, *completely different* technology to understand.
2. This second technology had a complex relationship to the first technology, and doing anything useful required a firm grasp on both.
3. This technology used a *completely different* syntax for expressing what it was meant to express.
4. There were now a whole bunch of *new words to learn*.

The first point was pretty easy to surmount. The second point was avoidable by omission (we just used tag-based selectors to begin with). But the third and fourth points really slowed people down.

It's not like they were insurmountable obstacles. People eventually learned enough of the CSS vocabulary and sytnax to do what they wanted to do, and then they moved on. What was interesting is that I would see the pattern repeat as we moved into each new area. They would understand the concept, and the relationship of the current concept to the others. But the rote ingestion of syntax and vocabulary would take time. Lots of time.

The thing that I noticed most, watching these people struggle to make their webpages look the way they wanted them to look, is just how much *random information* they needed to ingest. They needed to know that a link is, counterintuitively, represented by the tag <span class="mono">a</span> and not the <span class="mono">link</span> tag. They needed to remember that every CSS rule needs to end in a semicolon, or things fail silently. They needed to know about <span class="mono">float</span> and <span class="mono">clear</span> and the fact that <span class="mono">div</span> defaults to <span class="mono">display: block</span> but <span class="mono">span</span> doesn't. *And they were still dealing the easy stuff.*

So I think the first difficulty of programming could be summarized thusly:

***To make any sort of computer program, even a very simple one, the amount of random trivia you need to know is completely bananas.***

-------

Googling helps. And Stackoverflowing. However, they're not a panacea: for beginners, you have to know a certain amount to even search for answers effectively (it's sort of like how you need to know the fundamentals of spelling before you can look up a word in the dictionary). And for experts, no site on earth is going to help you manage the huge amount of information that you need to have in hand to deal with *your* project.

For this reason, getting better at programming doesn't make this problem go away. So if you're someone who programs a lot, you don't have to think twice about how to, say, iterate through a list in Python. It's in muscle memory, and pulling that factoid up doesn't consume much brainpower. However, you're forced to become aware of a multitude of other data points, all of which need to be available for recall at a moment's notice: the naming conventions for the project you're working on, the fact that method <span class="mono">foo</span> is really computationally expensive and shouldn't be called very often, the order of the parameters to the <span class="mono">Bar</span> constructor, and so on. 

As an analogy, this problem would be the equivalent of having to learn new vocabulary words for each document that you wrote in English. Some of them would have very similar meanings to other words that you knew, but would be spelled totally differently. Others would be spelled similarly, but have dramatically different meanings. Others would have the *exact same spellings*, but different meanings depending on the context. And there would be *thousands* of these words. And if this is a professional project, you're working on this document with hundreds of other people, each of whom are modifying the dictionary at will. And the definitions for each of these words are spread across thousands of different text files. And if you misuse a word, *things explode*.

OK, so, yeah, you have to know a lot of stuff in order to program. And this is pretty horrible. But! A lot of the pain of having to *know* is offset by our ability to *understand*. For example, if you can build up a mental model of how you've organized all the objects in your system, you don't have to store all of their names and locations in your short-term memory; you can simply query the mental model you've got built up. 

But here's the thing - understanding in programming is almost as difficult as knowing. And this will be the topic of part 2. 