+++
date = '2026-07-03T12:55:40+05:30'
draft = false
title = 'Electronics Enclosure - Purdue ROV'
weight = 1
+++

*August 2025 - Present*

**Goal:** To design and manufacture the electronics enclosure for the ROV (Remotely Operated Underwater Vehicle), ensuring structural strength, and reliable waterproofing. 

In August 2025, I joined the Purdue ROV (Remotely Operated Underwater Vehicle) team. This student-led team designs and builds underwater robots to compete in the annual MATE ROV World Championship. The tasks that this robot undertakes is stipulated by the competition and usually follow the theme of ocean ecosystem protection. 

{{< img src="rov/Full ROV Assembly.png" alt="Sketch" width="75%">}}

The 2026 competition, held in Newfoundland & Labrador, Canada, requires our ROV to operate in low-temperature ice tanks, high-velocity flume tanks, and saltwater offshore engineering basins so we had to design our ROV with these conditions in mind. 

#### Prerequisites for the Electronics Enclosure

1. The interface between the carrier plate and hat must be waterproof 
    - This is done by incorporating an O-ring and a groove
2. Carrier Plate should be Anodized Aluminum
3. The top hat needs to transparent, so the team leads decided that it should be SLA printed in [Formlabs Clear Resin](https://formlabs.com/global/products/clear-resin/)
4. The enclosure must be hydrodynamic, since it would protrude up out of the frame 
5. Include heatsinks and thermal pads for heat management of the Raspberry Pi and other boards 

#### Design

Previous years designs had an aluminum top hat and an aluminum carrier plate. We were retaining a similar design for the latter, only modifying the scaffolding for the new elecronics stack. 

I worked with a team member, Lauren, on the enclosure. She made the 3D model for the plate and I worked on the top hat. 

My initial design features for the hat were- 
1. Rounded corners and slanted sides 
2. Names of all team members embossed on the 
    - I chose to emboss instead of engrave so that the sturctural integrity doesn't get affected
3. Increased screws and reduced height (compared to Aluminum hat)

#### Iteration 

{{< img src="rov/Assembly1-rov.png" alt="Sketch" width="70%">}}

The above image shows one of my initial designs for the top hat. 
Dimensions were - 
1. Length: 10.7 in 
2. Width: 8.5 in 
3. Height: 5.5 in 

I got feedback during our team's annual design review with alumni and team leads. They recommended reducing the draft (angle), decreasing the height, and increasing the fillets around the corners. I made these changes to the design. 

{{< img src="rov/final-design.png" alt="Sketch" width="70%">}}


I also conducted FEA (finite element analysis) at 7.5m, to validate the thickness of the vessel. 

{{< img src="rov/fea.png" alt="Sketch" width="70%">}}

The final thickness was 0.26 in, and final height was 4.8 in. 

#### Manufacturing

Under usual circumstances, I would SLA print this on campus at Bechtel Innovation Design Center. However, the Form 4L was out-of-order and so I asked an Alumni working at Formlabs to print it for the team and mail it to us. 

Around the same time, Lauren finished carrier plate design and we needed to CNC Manufacture it on the Haas VF-4 Mill. I created the CAM on Autodesk Fusion. 

{{< img src="rov/CAM.png" alt="Sketch" width="70%">}}

During the CAM process we faced a few issues- 
1. The tool hit the tool clamp and broke 
2. Some of the toolpaths were time consuming, and so we had to finish the process over multiple days
    - This meant that probing the part was extremely important, to ensure high manufacturing precision

{{< img src="rov/CAM1.jpeg" alt="Sketch" width="65%">}}
{{< img src="rov/plate.jpeg" alt="Sketch" width="65%">}}

#### Assembly 

Once we recieved the top hat, we tested the interface and looked like it would work! 

{{< img src="rov/hatplate.jpeg" alt="Sketch" width="65%">}}

However, upon closer look there were other issues- 
1. The resin had warped, the bottom was not flat, and the overall size was smaller 
2. The o-ring groove on the carrier plate was also not completely flat, so the interface was not waterproof 

We tried hard to fix these issues. 
1. I tried to sand the hat down to size, but it would not close properly. 
2. Some other team members started the process of remanufacturing the plate 
3. As backup we also bought an off-the-shelf enclosure [(Polycase)](https://www.polycase.com/zq-100802#ZQ-100802-95) and drilled connector holes into it. 

#### Conclusion 

Ultimately, due to these issues we ended up using the Polycase enclosure. While this was not the most satisfying end to months of our hard work, I was made Structures Lead of Purdue ROV for the 2026-27 season. To prevent such issues from happening again, I started planning and designing along with the rest of the team over the summer. 






 