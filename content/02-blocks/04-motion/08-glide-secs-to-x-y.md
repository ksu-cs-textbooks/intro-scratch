---
title: "glide () secs to x: () y: ()"
pre: "8. "
weight: 80
---

![glide () secs to x: () y: () block](/images/glide-secs-to-x-y.svg)

The **glide to x: () y: ()** block moves a sprite to the coordinates (x, y) over the specified number of seconds, provided the coordinates are on the stage.  

#### Notes
* If the desired position has off-stage coordinates these will be clamped to the max/min allowable coordinate to keep the sprite on-stage. I.e. attempting to move a sprite to (6,300) would instead place it at (6, 180). The coordinate system for the stage is: 

![Scratch Coordinate System](/images/xy-grid.gif)