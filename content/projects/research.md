+++
date = '2026-07-03T12:57:07+05:30'
draft = false
title = 'Spherical Four-Bar Wing Mechanism - MARS Lab'
weight = 2
+++

*December 2025 - May 2026*

**Goal:** To design and build the spherical four-bar wing linkage mechanism for the tri-modal underwater robot (UR) for exploration of ice cavities. 

{{< img src="research/UR overiment annotated.png" alt="Sketch" width="75%">}}

In December 2025, I joined the MARS (Mechanisms And Robotic Systems) Lab as an undergraduate researcher to work on a low-cost underwater glider capable of extended mission in sub-ice ocean. Existing autonomous underwater vehicles (AUVs) are usually too large, power-intensive, and costly for deployment in such large and spatially constraints environments. This UR has drifting, gliding, and thrusting capabilities. 

My focus area, the wing mechanism, is adapted from a spherical four-bar mechanism. Fig. (a) shows the generic mechanism, while Fig. (b) presents our wing design. 

{{< img src="research/fig_sh.png" alt="Sketch" width="75%">}}

Each of the revoluting axes meet at a center point O, which forms a sphere around which all linkages rotate. This allows the wing to be in each of the required positions (folded back during drifting and deployed forward and tilted downward during gliding and thrusting) with only one actuator. This satisfies the multimodal qualities of the robot in an efficient manner by drawing lesser power from the battery. 

**Parameters:** I was given a rough CAD of the wings, and a brief explanation of the mechanism by my PHD student supervisor, Sheeraz. Along with that I was told to check and verify the CAD and then print and test it. 

{{< img src="research/wings_testing 1.png" alt="Sketch" width="75%">}}

#### Dry Testing

For this first test, I 3D printed the parts in PLA and connected it to a digital Multi Servo Tester. 

Some issues I faced were- 
1. The revoluting axes did not meet a common point in the middle, hence the movement was not smooth. 
2. The wings were not hydrodynamic. 
3. The linkages broke easily. 
4. The whole wing was too large to be 3D printed in one go.

My solutions were- 
1. I changed the CAD to make sure the linkage interfaces were flush with each other. I also verified that they all met at a single point
2. I modified the design to include shoulder screws and bearings for smoother rotation.
3. I used Onshape to make the wing the shape of a NCAA airfoil.
4. I reprinted the linkages in Onyx, a stronger carbon fiber and nylon composite.
5. I created a method for the wing to be printed in two parts, with an M2 screw in the middle.

{{< img src="research/shoulder screws.png" alt="Sketch" width="45%">}}

I conducted a few more dry tests without printing the full wing until I felt that the mechanism worked. 

{{< img src="research/partial wing.png" alt="Sketch" width="75%">}}
{{< video src="research/hand testing.mp4" alt="Sketch video" width="45%" >}}


#### Specifics 
 
The actuator of the system was a 55kg servo motor with M3 x 0.5 fasteners and nuts. The shoulder scews had 4mm shoulder diameter with a 10 mm shoulder length. The two halves of the wings were connected with M2 screws and nuts. 

#### Pool Testing 

Then we had our first pool test!! 

{{< img src="research/pool test 1.png" alt="Sketch" width="75%">}}

We learnt a few things from the pool test- 
1. The plastic placed directly on the output shaft gets worn out and eventually stops working 
2. The waterproof servo motor was not 100% waterproof to the depths we were taking the bot 
3. When the wings folded tilted downward too low, the torque of the motor ws not enough to pull it back into position.

{{< img src="research/UR in pool.jpeg" alt="Sketch" width="75%">}}

#### Iterating 

1. I looked into different servo horns to attach to the linkages. I settled on an Aluminum circular servo horn, because the teeth will not wear out easily. I adapted the the design to include this and made sure that the rotary joints still met at a single point. 
2. We did not have the time to build a servo enclosure so we used epoxy to waterproof the servo till a certain depth 
3. This challenge took a while to solve 
    - Initially I added stoppers on either side of the output link to prevent the wing from move past the point of return. This worked, but then we needed the wing to stay in that position while in the water. 
    - I tested small magnets on the supper and the output link, but the magnets were not strong enough to hold the wing in its horizontal position. 
    - Finally, one of my teammates came up with the idea of using an elastic to hold it down. This worked! 

#### More Pool Testing! 

Once we added these changes to the wing mechanism, we took the whole UR into the pool for multiple tests. This time we found no issues, and the wings worked as we expected. 
{{< video src="research/wings.mov" alt="Sketch video" width="90%" >}}

#### Research Paper 

This project spanned the months of January to March 2026 and after we completed validation, I co-wrote the research paper that we submitted to ASME. 

Currently, the paper has been approved for [IDETC-CIE 2026](https://idetc.secure-platform.com/a/solicitations/280/sessiongallery/24184/application/192073) conference in August where Sheeraz will be presenting our design! 
 
{{< img src="research/team picture.jpeg" alt="Sketch" width="75%">}}