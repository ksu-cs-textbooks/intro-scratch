---
title: "go to x: () y: ()"
pre: "6. "
weight: 60
---

![go to x: () y: () block](/images/go-to-x-y.svg)

The **go to x: () y: ()** block moves a sprite to the coordinates (x, y) provided they are on the stage.  

#### Notes
* The movement is instantaneous. If you would like it to be animated over time, see the **glide () secs to x: () y:()** block.
* If the desired position has off-stage coordinates these will be clamped to the max/min allowable coordinate to keep the sprite on-stage. I.e. attempting to move a sprite to (6,300) would instead place it at (6, 180). The coordinate system for the stage is: 

![Scratch Coordinate System](/images/xy-grid.gif)