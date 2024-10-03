---
title: "Sequence"
pre: "1. "
weight: 10
---

At the core, a program is simply a step-by-step set of instructions the computer will carry out. In Scratch, these instructions take the form of blocks, which snap together in a sequence, which we typically refer to as a block stack (or stack).

For a sequence to be executed (carried out), it must start with a "hat" block, so called because its shape resembles a baseball cap:

![Hat block shape](images/hat-block-shape.svg)

This block indicates the conditions that will trigger the execution of blocks that are snapped into place beneath it. The commands of these other blocks will be carried out in order - a *sequence*. For example, the following script will play the first two measures of the tune "Hot Cross Buns":

![Hot Cross Buns script](images/hot-cross-buns.svg)

Clicking the green flag will play each note in the order they appear in the sequence. You can see the full program [here](https://scratch.mit.edu/projects/1075943423) or run it below: 

<iframe src="https://scratch.mit.edu/projects/1075943423/embed" allowtransparency="true" width="485" height="402" frameborder="0" scrolling="no" style="margin: 0 auto; display: block;" allowfullscreen></iframe>

If we leave off the hat block, then the sequence of blocks will never be executed.  We call a stack without a hat block an *orphan* stack. 

Often, programmers will leave a sequence of blocks that they may come back to work on later orphaned intentionally, as they might comment out sections of code in another programming langauge. However, best practice is to remove orphaned code once you are sure it is no longer needed, as having many orphan stacks makes the script harder to read and understand. 

You can have multiple stacks in a Scratch program, and each will execute when its starting condition is met. For example, if two stacks both start with a **when flag clicked** block, *both* will run when the green flag is clicked. This is covered in more detail in the *paralleism* section.