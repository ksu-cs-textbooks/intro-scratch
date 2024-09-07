---
title: "set y to ()"
pre: "14. "
weight: 140
---

![set x to () block](/images/set-x-to.svg)

The **set y to** block changes the sprite's y position to the provided value.  

#### Notes
* The movement is instantaneous. 
* If you want to set both the x and y coordinates at the same time, use **go to x: () y: ()** instead.
* If the desired position has off-stage coordinates these will be clamped to the max/min allowable coordinate to keep the sprite on-stage. I.e. attempting to set y to 250 would instead set it to 180. The coordinate system for the stage is: 

![Scratch Coordinate System](/images/xy-grid.gif)