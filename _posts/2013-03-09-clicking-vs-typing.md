---
layout: post
title: "Clicking vs Typing"
description: "Thinking about methods of interaction"
category: 
tags: []
published: true
author: eli
---
{% include JB/setup %}

As computers are now, there are two main ways of interacting with them: **typing** and **clicking**. I think that examining these modes of interaction can yield some insight into making programming easier.

## Generation and Selection

Fundamentally, the big difference between the two is that typing is **generative**, while clicking is **selective**. You've got to have a lot of pre-existing knowledge in your head to type. Even if you're just writing English prose, for example, you have to know the rules of the language, the spellings of words, and so on. On the other hand, clicking doesn't require a lot of understanding. In fact, maybe it would accurate to say that typing *requires* understanding, while clicking *generates* understanding. By clicking around in a given environment, you can figure out what different things do.

What seems interesting to me is that more or less every programming environment in use today is predominantly typing-oriented. For most working programmers, it's usually a combination of:

![image](http://thoughtmachine.co/assets/themes/twitter/img/tm.png)

and:

![image](http://thoughtmachine.co/assets/themes/twitter/img/cli.png)

I'm not critiquing this fact - it makes a lot of sense. Most programmers have already done the hard work of accumulating the understanding necessary to use typing as their primary means of interacting with the computer. Additionally, it seems like typing is a much more efficient way of getting information into the computer. Lastly, typing fascilitates much "bigger" interfaces - the number of commands that one could type at the command line, for example, is much bigger than could ever be expressed as point-and-click options.

## Why click at all?

Typing is already pretty predominant in programming tools, so let's now explore the benefits of clicking. 

### Discoverable and Latent Interfaces

Clicking facilitates **discoverable** interfaces, while typing fasciltates **latent** interfaces. Each interface type has its place. Discoverable interfaces give the user information ahead of time, while latent interfaces give feedback once the user has done something:

![image](http://thoughtmachine.co/assets/themes/twitter/img/feedback-cli.png)

Because the set of options in a clickable interface needs to be finite (so they can all fit on the screen), it can be very fast for the user to gain feedback on the correct way to use the interface and figure out what each element does. On the other hand, [whole sites](http://www.bashoneliners.com/) exist to compensate for the complexity that arises out a latent interface. I've been using the command line for awhile, and I've probably used 10% of the total commands that come with OS/X. On the other hand, I clicked on every button in Illustrator within 20 minutes of installing the program.

### Information In, Information Out

Typing and clicking differ in terms of how they optimize for **information flowing** to and from the programmer. In the act of building any piece of software, there will be phases in which a lot of information is flowing from the programmer to the computer (think about those first giddy days of a project, when you're writing thousands of lines of code). There are also phases in which an equal amount of information is flowing from the computer back to the programmer (during debugging or testing, for example). Because clickable interfaces can rely on the entirety of the screen, their capacity to communicate information back to the programmer is much higher than typing interfaces. Conversely, due to the physical efficiencies of the act of typing versus moving a cursor all over the place, typing is a much more efficient way to getting information from a programmer's head into a computer.

### Focus and Exploration

The most salient different between the two modes of interaction is the type of mindset they accomdate best. Typing facilitates a **focussed** mindset, while clicking fascilitates an **exploratory** mindset. When you know exactly what you want to do and you want to do it quickly, typing is usually the best choice. If you want to poke around and figure out what's possible, clicking is usually the best choice.

As programmers, I think that we've come to hold the focussed mindset in much higher esteem than the exploratory mindset. Much has [been](http://psygrammer.com/2011/02/10/the-flow-programming-in-ecstasy/) [written](http://blog.ninlabs.com/2013/01/programmer-interrupted/) about the importance of the [flow state](http://en.wikipedia.org/wiki/Flow_state) for programmers. While I don't disagree that the flow state is an essential element of doing good work (for almost any job, not just programming), the idea that it can only look like intense periods of typing is a bit limiting.

Do we have any SimCity 2000 fans in crowd? Show of hands? I knew it. I know this sounds weird, but I think of SimCity as a classic example of a clickable-interface-driven, exploratory, flow-state experience.

![image](http://thoughtmachine.co/assets/themes/twitter/img/simcity.png)

SimCity play to the strengths of its clickable interface - lots of information is conveyed to the player; there's a small number of possible actions; feedback is given ahead of time to prevent the player from doing anything illegal; and the experience is highly exploratory ("What happens if I put a power plant next to the school?"). The basic elements are presented simply and are easy to manipulate with the mouse, but the results are excited and complex.

## Compromise

Luckily, programs don't have to choose to be entirely clickable or entirelly typing-driven. In fact, a blend of the two styles usually yields the best stuff. Some notable examples that spring to mind:

- **[Max/MSP](http://cycling74.com/products/max/)**: Max is a system that allows musicians to create "[patches](http://blog.soundsorange.net/wp-content/uploads/2006/09/SimpleMessageSystem.jpg)" using a visual, data-flow programming language. A great deal of information is represented in a 2-D grid, but much of the construction of patches can be done with the keyboard.
 
- **[Gmail's hotkeys](http://support.google.com/mail/answer/6594)**: This one might seem pretty quotidian, but I think it deserves to be called out. Gmail's comprehensive, customizable hotkey system lets people move really fast, while maintaining the benefits of a webapp (accessible from many devices, visually rich, cloud-hosted).

- **[NERDTree for vim](http://www.vim.org/scripts/script.php?script_id=1658)**: As a very visual person myself, it's enourmously helpful for me to have a way to "see" the directory structure of a given project. In this mode, using the mouse always makes the most sense to me, and I end up interacting with files and folders by clicking. Even though vim is built to be exclusively keyboard-driven, this exception to that principle makes me way more comfortable and efficient.

- **[Nethack's GUI](http://erapert.files.wordpress.com/2010/04/nethack2ot7.jpg)**: [Nethack](http://en.wikipedia.org/wiki/Nethack) is an extremely complicated terminal-based computer game. It definitely takes advantage of the "bigger" interfaces afforded by keyboard control - almost every key on the keyboard has an action associated with it (for example, pressing "q" will tell your character to quaff a potion, while pressing "Q" will tell your character to select an object for their quiver). What's interesting is that people have subsequently made [GUI wrappers](http://nethack.wikia.com/wiki/Graphical_user_interface) for the underlying engine. All of the keyboard commands still work, but certain [versions](http://erapert.files.wordpress.com/2010/04/nethack2ot7.jpg) surface the most common commands as clickable buttons. So, the important stuff is discoverable, while the expert-level stuff is latent.

## Food For Thought

- Notice the next time that you're in a high-input phase of your programming project (debugging, testing, etc). What sort of interface do you crave in those times?
- Similarly, notice the next time you're in an exploratory phase (for example, when designing architecture, or modeling behavior). What sort of interface feels best during those times?
- Which other programs blend different interaction styles well? Which use the wrong paradigm?
- Just for kicks, think about what a mostly-clicking command line would look like. How would you make it usable?
- Would it be possible to create a program editor that had variable levels of click-friendliness? For example, when you're just starting out with a language or framework, make the interface highly discoverable, then allow the user to make things more typing-oriented as they gain proficiency. What would that look like? Would it be better than what we have today?	



