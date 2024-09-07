---
title: "glide () secs to ()"
pre: "7. "
weight: 70
---

![go to](/images/glide-secs-to.svg)

The **glide () secs to ()** block moves the sprite to the specified location over the specified number of seconds.  Possible locations include:

* __random position__ - randomly chosen coordinates on-stage
* __mouse pointer__ - the location of the mouse cursor _at the moment this block is executed_
* The position of other sprites in the project _at the moment this block is executed_

#### Notes
* The names of other sprites only appear in the list after they have been added to the project
* When a sprite is chosen as the target, the position used is always that of the original sprite, not one of its clones