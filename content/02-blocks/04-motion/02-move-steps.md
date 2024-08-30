---
title: "move () steps"
pre: "2. "
weight: 20
---

![move () steps block](/images/move-steps.svg)

The **move () steps** blocks moves a sprite in the direction it is currently facing. Each step corresponds to one unit on the stage. 

#### Notes
* The movement of this block is immediate. If you want the movement to be animated over time, use a glide block or repeat the **move () steps** alternated with a **wait () seconds** block. See the [animated movement design pattern]({{% ref "/04-design-patterns/03-animated-move" %}}) for details.
* The direction of the sprite may not correspond with the artwork of the sprite. For example, Scratch cat is drawn facing to the left (90 degrees).
* If the block would move the sprite off-screen in one of the two coordinates, it will stop moving in that direction while still moving in the other. This causes the sprite to appear to "slide" along the edge of the screen.
