---
layout: home
title: Code and Experimental Testing
author_profile: true
classes: wide
---


### Ph.D Research: Stereo Camera Fiducial Tracker GUI
![image-center](/assets/images/stereo_test_setup.png){:width="520"}{: .align-left}
![image-center](/assets/images/fiducial_gui.png){:width="520"}{: .align-left}

Much of my and my lab's work involves testing and characterization of soft structures.  As these often perform a variety of motions and change in multiple degrees of freedom, typical materials testing machines often do not match the capabilities we need.  For my research, I have mainly needed to track the positions of various links, so I developed a system to allow me to easily and accurately track positions of my structures, then created a GUI to perform most of the computer vision analysis with some user inputs, so I could easily collect data and have undergraduate researchers assist with minimal coding required on their end.

---


### Ph.D Research: Controllable-Synergy Gripper in Simulation
![image-center](/assets/images/urdf1x.gif){:width="400"}{: .align-left}

My main research has focused on augmenting underactuated hands for prosthetics; underactuation simplifies hand complexity, but limits capabilities, so I am augmenting these hands by developing a soft robotic stiffening joint to increase controllability over hand motions. These soft structures were fully characterized experimentally so they could be simulated.  The Pybullet simulator was chosen as it was open-source and used by similar groups for robot control; however, as with most simulators, it is most accurate in simulating rigid bodies.  The proposed solution was to approximate each of the soft structures as a series of rigid components, modifying their control inputs to ensure the actual outputs of the simulated system would be similar to those of the real system.  This process had already been defined for compliant underactuated hands with more traditional components, so we expanded this to work with our system with some modifications, including nonlinear stiffness and transmission matrices.  Work is now being performed to create a motion planner and to optimize the control structure to make it as simplified as possible for a multi-fingered gripper.

---

### Ph.D Research: Wearable Assistive Upper-Arm Device
![image-center](/assets/images/single_instron.png){:width="300"}{: .align-left} A side project I worked on for my Ph.D research was in building a device to augment arm strength using pneumatic artificial muscles (PAMs). This involved mechanical testing of different components to see how they would interact in our system; system modeling, primarily of the PAMs to ensure we achieved the desired outputs; as well as the development of various controllers to ensure the sensors and actuators interfaced properly.  The low-level pneumatic system ran on an MSP microcontroller, which interfaced serially with a Raspberry Pi running ROS that ran the high-level controls and communicated wirelessly with the sensors on the subject.  The model was used to improve the mid-level controller that translated the user's desired position to pneumatic setpoints for the actuators.

---

### Graduate Internship--Nvidia: Reinforcement Learning for Grasping Thin Objects

<iframe width="112" height="63" src="https://www.youtube.com/embed/ReM3lVkcS2w?controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
*NOTE: This is not my video, just an example of similar work from  [Nvidia's developer blog](https://developer.nvidia.com/blog/introducing-isaac-gym-rl-for-robotics/)

During my Ph.D, I interned with Nvidia's Robotics Research group.  While there, I worked on an algorithm that taught their robotic hand to pick up thin objects, like coins, from a flat surface, by taking advantage of the properties of the hand's soft finger pads in Nvidia's Isaac Gym simulator.  The company was in the process of developing engines to simulate soft components, so I also got to help debug some of the engine's early issues.  With two other team members, I worked on simulating a new anthropomorphic robotic hand and framework for a 6-DOF arm, and used model predictive path integral control as a reinforcement machine learning algorithm.  While there, I learned about parallellization and GPU acceleration, algorithms for reinforcement learning, and practiced setting reward functions and avoiding some of their pitfalls.


---

### Undergraduate Research: Laser Eye Surgery Machine Testing
![image-center](/assets/images/database.jpg){:width="400"}{: .align-left}
![image-center](/assets/images/pattern_test.jpg){:width="400"}{: .align-left}

I worked with a lab developing laser micromachining of lenses into cornea or hydrogels (contact lens material). As a part of this group, I created a database system to interface with the group’s data analysis program, storing the data together and creating search and filter functions to enable comparisons of relevant trials. I also created an algorithm to position the laser machine’s distance from the hydrogel and orient it normal to the hydrogel’s surface based on changes in back reflection data that occurred at material interfaces, a task which was previously performed manually.

![image-center](/assets/images/transient_hydrogel_results.png){:width="365"}{: .align-left}
![image-center](/assets/images/hydrogel_shear.jpeg){:width="140"}{: .align-left}
![image-center](/assets/images/hydrogel_shear_results.png){:width="365"}{: .align-left}
I ran several independent studies for my undergraduate research.  In the first study, I determined the transient effects on refractive index when laser writing lenses into hydrogel.  I found significant changes in refractive index or amount of phase change over time, which meant the timing in testing the refractive index of these structures was extremely important. The other study determined how the shear modulus changed from the addition of the micromachined structures into hydrogels.

---
