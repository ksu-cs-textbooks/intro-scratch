---
title: "change y by ()"
pre: "13. "
weight: 130
---

![change y by block](/images/change-y-by.svg)

The **change y by ()** block changes the sprites y-coordinate by the supplied value.  For example, if the sprite was currently at y: 130, and the value of -10 was supplied to this block, the new value would be x: 120.

#### Notes
* The movement is instantaneous. 
* If the desired position has off-stage coordinates these will be clamped to the max/min allowable coordinate to keep the sprite on-stage. I.e. attempting to change a sprite's y position by -400 would instead set its y position to -180. The coordinate system for the stage is: 

![Scratch Coordinate System](/images/xy-grid.gif)