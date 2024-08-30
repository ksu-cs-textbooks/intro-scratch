---
title: "introduction"
pre: "1. "
weight: 10
---

The motion blocks control the motion of the sprite across the stage.  In working with these blocks, it is important to remember the coordinate system Scratch uses, which is based on Cartesian coordinates. These consist of two coordinates, the first is along the x-axis (horizontal), and the second along the y-axis (vertical). The boundary of the stage is from -240 to 240 on the x-axis, and -180 to 180 on the y-axis. This can be seen in the image below:

![Scratch Coordinate System](/images/xy-grid.gif)

Sprites are allowed to move anywhere on the stage, but cannot move off it (if you want your sprite to disappear off-stage, use the **hide** block from the Looks palette). Attempting to change a coordinate to a value off-stage will instead set it to the maximum/minimum value.

In addition to specifying movement using coordinates, sprites can also be moved forward. Each sprite has a direction it is facing, measured as an angle between 0 and 360 degrees. The angle 0 is straight up, and positive rotations are clockwise. Rather than specifying positive and negative rotations on blocks, Scratch uses a clockwise and counterclockwise arrow to indicate a change in direction.

{{% notice info %}}
While Scratch adopts the familiar Cartesian coordinate system from mathematics, it does not adopt the unit circle (with the angle 0 aligning with the postive x-axis and positive rotations in a counter-clockwise direction). Instead it adopts clockface-based angles, with 0 degrees corresponding to 12-o'clock position, and positive rotation matching in the direction of clock hand movement.
{{% /notice %}}