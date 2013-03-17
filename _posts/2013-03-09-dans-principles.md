---
layout: post
title: "Dan's Principles to Make Programming Easier"
category:
tags: []
author: eli
published: true
---

{% include JB/setup %}

Eli and I were both inspired by Bret Victor's <a href="http://worrydream.com/#!/InventingOnPrinciple">Inventing on Principle</a> presentation.  Not only does he reveal new, mind-expanding ways of writing code, but he extrapolates the fundamental concepts into a philsophy of how we should lead our lives.  He's our kind of dude.

Bret talks about his own life principle -- that creators need an immediate connection -- and encourages all of us to ask, "What's <i>my</i> principle?"  After a bit of navel gazing, I settled on a sufficiently lofty principle for myself: I want to help people reach their full potential.  I want to help people do all they are capable of.

But I don't want this because I'm a saintly do-gooder who dreams of world happiness.  I want it because I'm a cynic who despairs at the lost value in humanity.  Antoine de Saint-Exupéry said it more eloquently in <i>Wind, Sand, and Stars</i>, when he related his thoughts after a train ride through China, wondering whether -- in the right circumstances -- one of the children around him could grow into a Mozart:

> "When by mutation a new rose is born in a garden, all the gardeners rejoice. They isolate the rose, tend it, foster it. But there is no gardener for men. This little Mozart will be shaped like the rest by the common stamping machine. This little Mozart will love shoddy music in the stench of night dives. This little Mozart is condemned.
>
> "I went back to my sleeping car. I said to myself: Their fate causes these people no suffering. It is not an impulse to charity that has upset me like this. I am not weeping over an eternally open wound. Those who carry the wound do not feel it. It is the human race and not the individual that is wounded here, is outraged here. I do not believe in pity. What torments me tonight is the gardener's point of view... It is the sight, a little bit in all these men, of Mozart murdered."

Alright, then.  Having started this discussion in the stratosphere, let's bring it down to earth.  I want to use programming to help people do all they are capable of.  And to do that, we need to make it more accessible.  Here are some more practical principles for how I think we can do that:

## Discoverability

"You are standing in an open field west of a white house, with a boarded front door.
There is a small mailbox here."

Thus were the first words of Zork.  Those were the only instructions you were given before you could begin exploring the unknown world in front of you.

Programming should be the same.  You should be given just enough information to stumble your way through the dark, and the ability to find answers to light your way.  Frameworks should emphasize discoverability at their core, allowing you to interrogate objects and resources for their interfaces, letting you go down incorrect paths that teach you about the world even if they don't lead you to your destination.

## Composability

The world's finest creation tool will always be, for me, Legos.  So when it comes to imagining a perfect programming tool, I tend to gravitate back to the Lego metaphor.  In the same way Legos can come in 1x1 bricks that can be the fundamental building blocks of empires, or customized, specific molds to cater to special needs, so too should objects and frameworks be composable so you can construct them into wholes greater than the sum of their parts.  Small building blocks should snap together to become larger building blocks that can in turn be used to build ever-grander layers of abstraction.

Building blocks should fulfill Wikipedia's definition of composability:

+ self-contained (modular): it can be deployed independently -- note that it may cooperate with other components, but dependent components are replaceable
+ stateless: it treats each request as an independent transaction, unrelated to any previous request. Stateless is just one technique; managed state and transactional systems can also be composable, but with greater difficulty.

## Visibility

Programming is too opaque.  This never occurred to me until I read Bret Victor's post on [Learnable Programming](http://worrydream.com/#!/LearnableProgramming) and saw what it inspired in [LightTable](http://www.lighttable.com/).  One day soon I think we'll realize we've been programming blindly for the past 30 years.  Using a barebones text editor will feel as constraining as the punch cards of the 1970s.  Future programs will let you see your data, your objects, and all their interactions in real-time as you create them.

And just as data will be visible, so too will the structure of your code.  It pains me to work through directory hierarchies of assorted files of different types that all relate to a single project.  A project should be presented as a unified whole, and let me zoom into the parts I'm interested in.  Visibility, as it relates to programming, is not just about showing the hidden parts, but also about obscuring complexity so you can focus on only the pertinent pieces.

## Guidance

Finally, programming languages should follow a few rules to guide people who stumble through their darkness the best they can:

+   A language should make it easy to do the right thing and, conversely, hard to do the wrong thing.
+   A language should force specific and documented inputs and outputs with every interface.  It's crazy that it's 2013 and you can write a method with positional, non-obvious parameters and have no idea what's expected in return without reading the code.
+   A language should offer insanely helpful error messages.  Too often, parsers and compilers are written that treat error handling as an afterthought.  But, in fact, most of our interaction with them comes when they report an error state.  We should build them with the importance of error handling in mind -- or, better yet, build our IDEs to prevent most errors altogether (more on that in a future post).

Unlike Bret Victor, I have no implementations to show for my lofty ideals -- yet.  But I lay out these programming language principles here to help guide me as I try to discover or build a more perfect tool to bring more Mozarts into this world.
