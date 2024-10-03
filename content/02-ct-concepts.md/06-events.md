---
title: "Events"
pre: "6. "
weight: 60
---

In programming, an event triggers the execution of code. You've already worked extensively with one event in Scratch, the **when flag clicked** block:

![when flag clicked](images/when-flag-clicked.svg)

Clicking the green flag button on the stage triggers the hat block to execute. 

A related event is triggered when you click the red stop sign button. That button stops all running scripts, effectively stopping the program. You can also trigger this event with the **stop ()** block:

![stop ()](images/stop.svg)

In addition to stopping all scripts in the program, the **stop ()** block can be used to stop the other scripts of this sprite, or the specific script it appears in.  

There are many other events and blocks that interact with them in Scratch. Let's examine each.

## User Events

User events are events triggered in some way by the user. The green flag is the most common example - clicking it will execute any stack of blocks starting with a **when flag clicked** block:

![when flag clicked block](images/when-flag-clicked.svg)

Likewise, the **when () key pressed** block will execute its block stack when the specified key is pressed. You can set it to the arrow keys, letter keys, space, or 'any' key:

![when () key pressed block](images/when-key-pressed.svg)

You can also use the **when this sprite clicked** block to trigger a stack of blocks when the user clicks on its sprite.

![when this sprite clicked](images/when-this-sprite-clicked.svg)

Finally, a unique event in Scratch is represented by the **when [loudness] > ()** which will trigger when a microphone attached to the computer detects sound louder than the specified threshold:

![when [loudness] > () block](images/when-loudness-greater-than.svg)

## Timer Events

Scratch includes a timer that starts when the green flag is clicked, and counts up in seconds. Its value can be accessed with the **timer** reporter block, and it can be restarted with the **reset timer** block. Both are found in the *Sensing* palette.

![timer](images/timer.svg)

![reset-timer](images/reset-timer.svg)

In addition to these two blocks, the **when [timer v] > ()** block can be used to trigger a block stack when the timer reaches a certain value, i.e. 10 seconds:

![When timer > 10](images/when-timer-greater-than.svg)

## Backdrop Events

The **when backdrop switches to ()** block triggers when the backdrop is changed to the selected value:

![when backdrop switches to ()](images/when-backdrop-switches-to.svg)

This can be especially helpful when a program is organized as a _state machine_ with each backdrop representing a different state. One example of this approach would be an animated storybook with each backdrop serving as a new "page" of the story.

## Clone Events

When a new clone is created it executes any block stacks starting with the **when I start as a clone** hat block:

![when I start as a clone](images/when-i-start-as-a-clone.svg)

## Broadcast Events

Finally (and perhaps most powerfully), the programmer can create custom events in Scratch using the **broadcast ()** or **broadcast () and wait** blocks.  These blocks send a message that executes any corresponding **when I receive ()** hat blocks:

![when I receive ()](images/when-i-receive.svg)

A new message can be created by selecting the "New message" option in any of these block's selection menus:

![new message option](images/new-message-option.png)

The **broadcast ()** block sends the corresponding message and immediately continues executing blocks in its own stack:

![broadcast ()](images/broadcast.svg)

In contrast, the **broadcast () and wait** sends the message and then pauses its stack's execution until all **when I recieve ()** stacks have finished executing: 

![broadcast () and wait](images/broadcast-and-wait.svg)

Note this does not necessarily mean the entire stacks are executed before the pause ends, as the other stacks will pause at **wait () seconds** and at each loop iteration. See the *parallelism* section for more details.