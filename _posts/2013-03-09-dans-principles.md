---
layout: post
title: "Principles to Make Programming Easier"
description: Simplicity, Discoverability, Composability, Visibility, Guidance
category:
tags: []
author: dan
discoverable: true
published: true
---

{% include JB/setup %}

Let's talk about principles.

Eli and I were both inspired by Bret Victor's [Inventing on Principle](http://en.wikipedia.org/wiki/Type_introspection) presentation.  Not only does he reveal new, mind-expanding ways of writing code, but he extrapolates the fundamental concepts into a philsophy of how we should lead our lives.  He's our kind of dude.

Bret talks about his own life principle -- that creators need an immediate connection -- and encourages all of us to ask, "What's <i>my</i> principle?"  After a bit of navel gazing, I settled on a sufficiently lofty principle for myself: I want to help people reach their full potential.  I want to help people do all they are capable of.

As the importance of technology, data, and information grows, knowing how to code becomes an important way to make your life better.  And therefore coding becomes a means of reaching your full potential.

In order for more people to learn how to code, we need to make coding itself more accessible.  Below are some principles for how I think we can do that, whether through frameworks, tools, or the languages themselves (which one day may all merge into one).

## Simplicity

I think simplicity lies at the core of accessibility.  Sadly, as [Eli's post pointed out](/what-makes-programming-hard-pt-1/), to get even a rudimentary modern website up and running requires a knowledge of a baffling array of technologies.  Although I love the sensible and practical abstractions that modern MVC frameworks have introduced, I miss the stark simplicity of what was, for many of us, our first dynamic web page:

    #!/usr/bin/perl

    print "Content-type: text/html\n\n";
    print "Oh golly, I made a dynamic web page!";

These days, complexity seems to be multiplying: modern Javascript frameworks create an MVC model within the browser that more likely than not talks to an MVC model on the server, with clever contraptions to keep the two in sync.  It all seems wonderfully magical, but to a novice it's an impenetrable jumble of abstractions.

My favorite example of elegant simplicity lately is [dreamer](https://github.com/dchester/dreamer-example), written by my co-worker David Chester.  Dreamer lets you write out a data model in Markdown and automatically generates a RESTful web service from it.  Without having to understand databases or web programming, a novice can start exploring RESTful architectures and data models.

## Discoverability

> "You are standing in an open field west of a white house, with a boarded front door.  There is a small mailbox here."

Thus were the first words of [Zork](http://en.wikipedia.org/wiki/Zork).  Those were the only instructions you were given before exploring the unknown world in front of you.

Programming should be the same.  You should be given just enough information to stumble your way through the dark, and the ability to find answers to light your way.  Frameworks, tools, and even languages should emphasize discoverability at their core, allowing you to interrogate objects and resources for their interfaces, letting you go down incorrect paths that teach you about the world even if they don't lead you to your destination.

As a simple example, every RESTful service at Shutterstock (where I work) has a /resources resource, that shows the complete interface for the service.  A programmer only has to know the hostname of a service to start exploring and using it.

Another example is [type introspection](http://en.wikipedia.org/wiki/Type_introspection), which lets developers examine an object at run-time.  Current implementations of this are minimal at best, often just showing lists of an object's methods or attributes.  But we can imagine an approach that's more tightly coupled with documentation and lets a developer learn about an object more deeply via an interactive interface.

## Composability

The world's finest creation tool will always be, for me, Legos.  So when it comes to imagining a perfect programming tool, I tend to gravitate back to the Lego metaphor.  In the same way Legos can come in 1x1 bricks that can be the fundamental building blocks of empires, or customized, specific molds to cater to special needs, so too should objects and frameworks be composable so you can construct them into wholes greater than the sum of their parts.  Small building blocks should snap together to become larger building blocks that can in turn be used to build ever-grander layers of abstraction.

Object inheritance held out the promise of creating complex structures from simpler building blocks, but has instead often led to brittle hierarchies and confusing dependencies.  Mixins are proving to be a more flexible way of combining bits of code, but can lead to discoverability problems when it's unclear where a method originates.  There's more work to be done to create a standard approach to composability within languages.

An oft-cited example of composability that can inspire us is the Unix command line.  By defining two simple communication streams -- in and out -- and a method for chaining programs together, it's possible to combine many simple Unix utilites to create fantastically complex functionality.

## Visibility

Programming is too opaque.  This never occurred to me until I read Bret Victor's post on [Learnable Programming](http://worrydream.com/#!/LearnableProgramming) and saw what it inspired in [LightTable](http://www.lighttable.com/).  One day soon I think we'll realize we've been programming blindly for the past 30 years.  Using a barebones text editor will feel as constraining as the punch cards of the 1970s.  Future programs will let you see your data, your objects, and all their interactions in real-time as you create them.

And just as data will be visible, so too will the structure of your code.  It pains me to work through directory hierarchies of assorted files of different types that all relate to a single project.  A project should be presented as a unified whole, and allow a developer to zoom into the relevant bits.  Visibility, as it relates to programming, is not just about showing the hidden parts, but also about obscuring complexity so you can focus on only the pertinent pieces.

## Guidance

Finally, programming languages should follow a few rules to guide people who stumble through their darkness the best they can:

+   A language should make it easy to do the right thing and, conversely, hard to do the wrong thing.
+   A language should force specific and documented inputs and outputs with every interface.  It's crazy that it's 2013 and you can write a method with positional, non-obvious parameters and have no idea what's expected in return without reading the code.
+   A language should offer insanely helpful error messages.  Too often, parsers and compilers are written that treat error handling as an afterthought.  But, in fact, most of our interaction with them comes when they report an error state.  We should build them with the importance of error handling in mind -- or, better yet, build our IDEs to prevent most errors altogether.

Unlike Bret Victor, I have no implementations to show for my lofty ideals -- yet.  But I lay out these programming language principles here to help guide me as I try to discover or build a more perfect tool to help people realize their ambitions.
