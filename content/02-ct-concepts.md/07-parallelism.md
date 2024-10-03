---
title: "Parallelism"
pre: "7. "
weight: 70
---

Parallelism refers to doing more than one thing _in parallel_ (at the same time). When we have two stacks of blocks both starting with a **when flag is clicked**, these both trigger thier execution when the green flag button is clicked, and appear to execute at the same time. Likewise, two stacks starting with **when I recieve ()** blocks listening for the same message will be triggered at the same time.

Parallism exists between stacks of blocks in the same Sprite, and also between all Sprites (and the Stage) - essentially any time an event occurs, each corresponding hat block will execute.

## Ordering and Synchronization

However, there *is* some order to parallel actions in Scratch. Consider these scripts:

![parallel say and think block stacks](images/parallel-say-think.svg)

The sprite containing them can only display *one* of the speech/thought baloons at a time, so one of these will take precidence over the other. Generally, they will execute in the order the stacks were created, but there is no guarantee of this.

Establishing an order to script execution is called _synchronization_, and there are several techiques we can employ.

### Yielding in a Stack

One of the easiest is to add a **wait (0) seconds** block in the stack we want to go last. A wait block pauses the execution of the current stack, and allows other stacks to finish their execution. Setting the seconds to 0 means that the pause is infantesmally small, but it does allow the other block stacks to run first (we call this a *yield* in computer science). In Scratch, loops also yield after each iteration.

While this approach works, it is not exactly intuitive, and it only ensures ordering between two stacks. However, it is important to know, as it can help understand the behavior of parallel stacks.

### Message-based Synchronization

A far more powerful approach is using **broadcast ()** and **when I recieve ()** blocks to trigger stacks in sequence. For example, the following script first executes the **say () for () seconds** block, then triggers the **think () for () seconds block**:


While the example is trivial, this appraoch to synchronizing parallel stacks is extremely powerful. You can have multiple stacks in multiple sprites triggered by each message, and you can define as many messages as you need.

One common design pattern using this approach is the [Get Ready and Go Design Pattern](), which helps ensure all sprites start in the expected state when a Scratch program is run.