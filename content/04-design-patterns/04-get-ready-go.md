---
title: "Get Ready and Go"
pre: "4. "
weight: 40
---

Sprites in Scratch maintain thier state - which means that if the program was stopped with a sprite in a certain position, the  next time the program is run, it will begin in that position. But for many Scratch projects, we want every sprite to start in a known position, regardless of where it last was.

One common pattern to accomplish this using messages is the *Get Ready and Go design pattern*. This pattern helps ensure that all sprites start at the intended position on stage, with the desired visibility, size, and effects *before* the program continues.

In this design pattern, a **broadcast () and wait** block triggers the initialization sequence by broadcasting a `Get Ready` message, and waits until all **when I receive ()** stacks finish their work before using a **broadcast ()** block to send a `Go` message (note, the names of the messages can be anything, "Get Ready" and "Go" were chosen for the ease of understanding thier meaning). The script looks like:

![initialize design pattern triggering sequence](images/get-ready-and-go-broadcast-stack.svg)

This script is often placed in the Stage (as it is more central to the program than sprites).  Then, individual sprites (and the stage) can listen for the two messages with **when I recieve ()** to trigger thier corresponding Get Ready and Go routines, i.e.:

![initialize and begin sprite stacks](images/get-ready-and-go-sprite-stacks.svg)


