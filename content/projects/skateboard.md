+++
date = '2025-07-12T23:18:19+05:30'
draft = false
title = 'Skateboard'
weight = 1
+++

In the Summer of 2025, during my internship at ATI motors, I built a prototype of an intelligent fork for pallet transportation. "Skateboard" is a nickname given to the project. 

{{< img src="files/Final-skateboard.jpg" alt="Sketch" width="60%">}}

The skateboard’s key advantage over pallet movers and similar machines is its ability to move omnidirectionally and perform zero-radius turns. This increases positional accuracy and could potentially save time and space. It would also use an electronic differential rather than a mechanical one, which is more compact and precise. 

For this project, I used Onshape for CAD work, SimScale for FEA analysis, and the Arduino IDE for hardware tasks. Most of the parts were either 3D print, laser cut, or machined. 

Before I began, some components like the motors, encoders, pulleys, and microcontrollers had already been selected. I was also given the following the design constraints- 
1. Test the motor before beginning designing and assembly
2. Make the unit as compact as possible 
3. Use 80 mm diameter wheels 

To fit the existing setup, I designed my own GT2 pulleys, and other parts for the electronic differential unit. 

{{< img src="files/Pulley-skateboard.png" alt="Sketch" width="30%">}}
{{< img src="files/Unit-skateboard.png" alt="Sketch" width="90%">}}

Through this process, I learnt how to CAD sheet metal parts, and got many of my designs laser cut and welded. 

After designing the complete assembly and sending parts to either get manufactured or 3D print, I worked on the electronics. 

{{< img src="files/Assembly-skateboard.png" alt="Sketch" width="80%">}}

The circuit consisted of a stack of an Arduino and two Motor Driver Shields that powered and controlled the 4 motors using data from Quadrature Encoders. I wrote a PID-based code, that monitored ticks and position of the wheels' rotations. 

Then, I started exploring different methods to communicate with the microcontroller system. My options were- 
1. Blynk (an IOT platform)
2. MQTT
3. Wi-Fi communication over a flask server 

I chose the third option and ran a webserver on my laptop to control the Arduino with an ESP32. To validate my code and set up, I created a test bench with the motors and all electronic components.

{{< img src="files/Bench-skateboard.jpg" alt="Sketch" width="80%">}}

I then moved on to assembling all the parts, which had been manufactured by this time. During this process, I realized that the foam board was to weak to hold the weight of the motors. So, I cut and drilled holes into a piece of scrap metal instead.  

{{< img src="files/Wheels-skateboard.jpg" alt="Sketch" width="80%">}}
{{< img src="files/Final2-skateboard.jpeg" alt="Sketch" width="80%">}}

I faced some issues with the 3D printed parts breaking, but after some changes and reprinting, I was able to run it on the ground and test my code and other ideas. 

{{< video src="files/Video-skateboard.mp4" alt="Sketch video" width="80%" >}}

With the design approved, I moved on to getting all the parts manufactured using metal. This meant modifying some of the designs for better manufacturability. 

{{< img src="files/Laser-skateboard.png" alt="Sketch" width="60%">}}

{{< img src="files/Final3-skateboard.jpg" alt="Sketch" width="60%">}}

I was not able to do much more because my internship came to an end. However, over the 3 months working at ATI Motors, I enjoyed the learning process and it was gratifying to see the working final product. I look forward to taking up more challenging and interesting projects like this!