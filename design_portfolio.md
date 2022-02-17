---
layout: home
title: Design Portfolio
author_profile: true
classes: wide
---

### Ph.D Research: Controllable-Synergy Grippers
![image](/assets/images/StiffeningDesigns.gif){:width="400"}{: .align-left}
My main research has focused on augmenting underactuated hands for prosthetics; underactuation simplifies hand complexity, but limits capabilities, so I am augmenting these hands by developing a soft robotic stiffening joint to increase controllability over hand motions. The design has had many iterations, including designs based on granular jamming, on increasing the cross-sectional area when pressurized, and on pure pressurization opposing bending. The final design (bottom right) involves a strain-limited cylindrical chamber in parallel with a stiffer strain-limited flexure; pressurizing the chamber significantly increases its stiffness, opposing the bending of the rigid links around it. The flexure mitigates the effects of chamber buckling on overall link motion, a major issue in previous designs. A paper using one of the earlier prototypes with a sonomyography-based sensor for real time prosthetic control is [here](https://ieeexplore.ieee.org/abstract/document/9176483).

![image-center](/assets/images/Robosoft_gripper.png){:width="400"}{: .align-right}
The developed controllable-stiffness joints were placed in series to create fingers, and a parallel gripper was created to demonstrate the effects of the joints. Three-joint fingers were selected based on the range of motion and stiffening properties of the joints. The link lengths and relative angles were optimized to take maximum advantage of the joints, such that the link placements could be maximally controllable when close to contacting an object. The gripper proved effective in grasping more objects and increasing the acquisition areas of objects when utilizing the stiffening joints, effectively improving the capabilities of the gripper [[link](https://ieeexplore.ieee.org/abstract/document/9115995)]. Further work is being performed to fully and accurately simulate the gripper for motion planning and control optimization in a multi-fingered gripper.


![image-center](/assets/images/Robosoft_grasps.png)

---

### Ph.D Research: Wearable Assistive Upper-Arm Device
![image-center](/assets/images/semiflextech_photorealistic.jpg){:width="500"}{: .align-right}
Another project I worked on for my Ph.D research was in building a device to augment arm strength using pneumatic artificial muscles (PAMs). Because of the varying and limited space available on the subjects' arms, we  elected to place the PAM's in a backpack, where they could generally be longer and be consistent subject-to-subject. Available length was particularly important as contraction length was only dependant on PAM length. To improve this somewhat, we developed a method to put the PAM's in series folded about a pulley; the advantages were mitigated by the amount of cable required and the non-contracting ends of the PAM's, but it did still give a significant improvement in contraction length. I also had to design a frame for the backpack to hold these PAMs and resist their contractions;
![image-center](/assets/images/semiflextech_fea.jpg){:width="400"}{: .align-left}
 for the 3 DOF's we wanted to assist, and 2 sets of antagonistic folded-series PAMs for each DOF, that meant the frame had to hold 12 PAMs, which each had contraction forces up to 600 N. Further, the components in the backpack had to be reasonably sized, as light as possible for the target users of elderly or disabled people, fully encase the backpack to prevent interference or injury from the soft pneumatic components, and be radio-frequency transparent as much as possible, to not interfere with the wireless sensors.  So the proposed frame was made almost entirely of different plastics, with hardened stainless steel shafts at the base to hold the pulleys, which saw the highest forces.

---

### Ph.D Research: 3D Printing Flexible Joints into Robotic Fingers
![image-left](/assets/images/printed_finger.jpg){:width="400"}{: .align-left}Elastomeric flexures are often used for relatively easy and inexpensive manufacturing of underactuated hands, commonly fabricated via Shape Deposition Manufacturing (SDM) or other casting techniques. I performed a brief study in the efficacy of multi-material printing these flexures simultaneously with the rigid components, varying printer settings, material interfaces, and print orientations for the best results. The commonly used dogbone-shaped flexure interface proved ineffective in this case as the material would stretch and pull out of its seating. As there was significant internal cohesion inside the flexible segments, a P-shaped interface was designed where the rod
![image-right](/assets/images/printed_flexure_fatigue.gif){:width="500"}{: .align-right} through the loop of the 'P' anchored it to the rigid segments, also giving high overall interface area and allowing the flexure to be positioned toward the back of the link. These fingers held up to fatigue testing of 1000 cycles with no noticeable changes. This method was also much faster than SDM or similar techniques as cure time was eliminated.

---



### Undergraduate Senior Design: Sample Automation
![image-left](/assets/images/SeniorDesign_tray.jpeg){:width="300"}{: .align-left}
![image-left](/assets/images/SeniorDesign_tubes.jpeg){:width="200"}{: .align-left}
 Myself and four team members designed a device to take treated blood analysis caps from provided trays and stack them into provided cartridges for the company Ortho Clinical Diagnostics. This was made difficult by the small spacings between caps in the trays and cartridges, and the fact that we had to manufacture all custom components ourselves.
![image-left](/assets/images/SrDesign_filter.jpeg){:width="400"}{: .align-right} We designed a device that flipped over the inserted tray and moved it across a 3D-printed ramped filter, which rearranged the caps to the spacing and radial orientation of the cartridges and then dropped them into stacks in a silo. The device then rotated the silo and pistons pushed the stacks of caps into the cartridges, keeping them in place with stoppers. The real-world implementation of the device had a low success rate for cap transfer; more precise component machining and more sensors were necessary for better control of the device.

![image-left](/assets/images/SrDesign.gif)

---


### Undergraduate Mechanical Design: Bottle Cap Redesign
![image-left](/assets/images/bottleCap_design.png){:width="320"}
![image-left](/assets/images/bottleCap_fea.jpg){:width="320"}
![image-left](/assets/images/bottleCap_FEAResults.png){:width="300"}{: .align-left}

A course project was to redesign and improve a common object. I redesigned the disposable plastic water bottle cap to be easier to open for people with arthritis or similar issues, comparing it both to the “eco-slim” style of bottle cap, and the older, larger style. The bottle cap industry is well-documented, so the materials and equivalent torques were well defined for FEA. My redesign involved changing the circular cap to a triangular one, both to reduce slip and to increase moment arm while turning. My design had a margin of safety of 1.1, and was 62% more volume than the eco-slim caps and 30% more than the older style, but with the savings of the rest of the eco-slim bottle, would cost 32% less to produce than the older style of bottle.

---

### Undergraduate Mechanical Design: Balsawood Bike Fork
![image-left](/assets/images/TrussDesign.jpeg){:width="450"}
![image-left](/assets/images/TrussCAD.png){:width="450"}

Myself and two team members worked to design, analyze, and build a balsawood truss structure representing a bicycle fork, with the goal of having the greatest strength-to-weight ratio. After competing between ourselves to design the strongest and lightest single-side of the fork structure, my base design was chosen and my teammates helped iterating FEA for different link sizes and in determining where to place the connecting links. Our final strength-to-weight ratio from FEA was 1448, one of the highest in our class.

---

### REU at Oregon State: Ankle Actuation for Cassie Robot

![image-left](/assets/images/CASSIE.png){:width="400"}{: .align-left}
Myself and a team-member were tasked with designing a fluidic actuation system for the ankle of the Cassie robot, in order to move more of the weight onto the main body of the device for decreased inertial loads. Several McKibben-style and piston actuators were tested to attempt to achieve the high-torque outputs required, and a pump was designed for this system. Overall, the system was heavier
and more complex in implementation than a simple push-rod and motor at the ankle and was not implemented in the robot.

![image-left](/assets/images/REU_PAM.jpg){:width="255"}{: .align-left}
![image-left](/assets/images/REU_testSetup.jpg){:width="210"}



### REU Part 2: Gerotor Pump
![image-left](/assets/images/pump_profile.jpeg){:width="270"}
![image-left](/assets/images/pump_moving.gif){:width="260"}
![image-left](/assets/images/pump_parts.jpeg){:width="380"}

I designed a pump to pressurize mineral oil to work with antagonistic fluidic actuators. A gerotor design was selected so the pump would be completely reversible, could provide constant flow per revolution, and would not require external dynamic seals.
The tooth profiles were optimized to provide the maximum compression per revolution, and the gear thickness was generated such that the pump could reach the calculated required flowrates for the fluidic actuators with the chosen motor.

![image-left](/assets/images/pump_manufactured.jpeg){:width="480"}
![image-left](/assets/images/REU.gif){:width="440"}

The pump was professionally manufactured from aluminum and Delrin parts and assembled in-house. Flowrates and RPMs were lower than expected, partially from incomplete bleeding or leaks in the system, but also likely due to additional drag on motor from being fully submerged in oil, high resistance due to the thin transmission tubing required for use in the system, and likely high and varying torques from the high compression per tooth. A design with more teeth and higher RPM’s would likely have worked more efficiently due to these considerations.

---
