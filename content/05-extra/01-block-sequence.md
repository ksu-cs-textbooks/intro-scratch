---
title: "Block Sequences"
pre: "1. "
weight: 10
---

The term sequence in computational thinking refers to issuing one command after another, to be carried out in order.  In Scratch, this is represented by a stack of blocks that have been snapped together. Each stack starts with a _hat block_ (so called becuase it resembles a baseball cap) that identifies the conditions that will start the execution (the carrying out) of that sequences's commands. You will learn more about hat blocks in the events chapter, but for now we'll only use the 'Green Flag Clicked' block:

![Green Flag Clicked](/images/green-flag-clicked.svg)

This particular block will start the execution of a stack of blocks beneath it when the Green Flag button on the stage is clicked (like the play button on a DVD player). Notice the tab projecting out of the bottom of the block? We can connect any block with a corresponding divot in its top. For example, we can connect a 'Say' block: 

![Say Block Example](/images/say-block-example.svg)

And when we click the green flag, this script will play, making Scratch the Cat (or whichever sprite this code belongs to) say the phrase "Hello":

![Say Hello Example](/images/say-hello-example.png)

We can add any number of blocks to a block sequence, and they will be executed one at a time.  We could expand the previous example to be:

![Longer block sequence example](/images/longer-block-sequence-example.svg)

And we might expect the result to look like this:

![Longer block sequence expected result](/images/sequence-example-animation.gif)

But if you create the above program in Scratch, you will only see the Scratch Cat speak phrase "I hope you enjoy learning to program".  Why?

Actually, Scratch _is_ making Scratch the Cat say all three phrases, and doing so one after the next. But it carries out these instrucions as quickly as it can. That means that the phrases "Hello!" and "Welcome to Scratch" are displayed on-screen for exactly 1 frame each (about 1/60th of a second for most computers). This is too fast for the human eye and mind to catch, so it seems like Scratch is skipping to the last phrase.

This is one of the important aspects of learning to program - the computer's understanding of our instructions is exacting, and does not necessarily line up with what we might expect if we gave the same instructions to another human being. We have to learn to adjust our understanding to how a computer operates to be able to write programs that do what we want. 
