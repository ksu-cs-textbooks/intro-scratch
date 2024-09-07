---
title: "set x to ()"
pre: "12. "
weight: 120
---

![set x to () block](/images/set-x-to.svg)

The **set x to** block changes the sprite's x position to the provided value.  

#### Notes
* The movement is instantaneous. 
* If you want to set both the x and y coordinates at the same time, use **go to x: () y: ()** instead.
* If the desired position has off-stage coordinates these will be clamped to the max/min allowable coordinate to keep the sprite on-stage. I.e. attempting to set x to -300 would instead set it to -240. The coordinate system for the stage is: 

![Scratch Coordinate System](/images/xy-grid.gif)