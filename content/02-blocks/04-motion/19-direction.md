---
title: "direction"
pre: "19. "
weight: 190
---

![direction block](/images/x-position.svg)

The **direction** block reports a sprite's current direction, an angle between -180 and +180 degrees.

#### Notes
* Setting an angle larger or smaller than the bounds will wrap (i.e. 185 will become -175)
* The value can be displayed on the stage by checking the box next to the block in the code palette
* The value displayed on the stage is always that of the original sprite
* When used in a script run by a clone, it refers to the clone's position