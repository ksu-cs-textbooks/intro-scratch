---
title: "change x by ()"
pre: "11. "
weight: 110
---

![change x by block](/images/change-x-by.svg)

The **change x by ()** block changes the sprites x-coordinate by the supplied value.  For example, if the sprite was currently at x: 110, and the value of 10 was supplied to this block, the new value would be x: 120.

#### Notes
* The movement is instantaneous. 
* If the desired position has off-stage coordinates these will be clamped to the max/min allowable coordinate to keep the sprite on-stage. I.e. attempting to change a sprite's x position by 600 would instead set its x position to 240. The coordinate system for the stage is: 

![Scratch Coordinate System](/images/xy-grid.gif)