---
title: "Animated Move"
pre: "3. "
weight: 30
---

The **move () steps** immediately moves a sprite the specified number of steps. But what if we want that movement to be slower, animated over time?  The various glide blocks provide smooth movement, but not in the direction the sprite is facing. Instead, we can emulate this movement with a combination of **repeat ()**, **move () steps**, and **wait () seconds** blocks:

![Repeat-Move-Wait design pattern](/images/repeat-move-wait.svg)

The total number of units moved is the product of the number of repeats and the movement in the block (i.e. repeating a movement of 2 units five times is $$2 * 5 = 10$$ total units moved). The value of the **wait ()** block determines how fast the sprite moves. A small value (i.e. 0.06, roughly 1/16 a second) will give good results.

A slighly more sophisticated version adds sprite animaiton, swapping frames each step forward:

![Repeat-Move-Wait-Next-Costume](/images/repeat-move-wait-next-costume.svg)


