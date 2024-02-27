---
layout: home
title: Code and Experimental Testing
author_profile: true
classes: wide
---

### ARA: Mobile Manipulation with Fanuc Arm

One of the main projects I worked on at ARA was in integrating a Fanuc arm onto a robotic ground vehicle platform, and creating a motion planning system for autonomous or teleoperated pick-and-place of high-mass payloads with a hook gripper.  The robotic ground vehicle used ROS for its autonomy structure, so the first challenge was in getting two-way communication between the Fanuc arm and ROS nodes to be functional.  There were minimal existing implementation for other Fanuc arm models into ROS,  and with some modification and updates to the arm model files I was able to achieve communication through a socket into ROS.  From there, I used existing MoveIt integrations for the main motion planning, tuning parameters for better performance and hard-coding speficifc waypoints and constraints to generate and save the proper trajectories to achieve the hooking motion required for grasp acquisition.  For the teleoperated strategies, I worked to make the controls as intuitive as possible for the operator by giving them control over end-effector position rather than joint angle and minimizing the DOF's they had to control to only three dimentsional position and hook rotation. The existing MoveIt joystick or servoing applications were not fast and configurable enough to realize these goals, so instead I ran my own minimized inverse-kinematics calculations to directly output custom joint trajectories based on the user's inputs.  As this bypassed MoveIt's planning and collision detection, I also implemented my own solution to that, imposing position and conditional joint limits to prevent collisions between the arm, payload, and vehicle in teleoperation mode. 

---


### ARA: Ground Vehicle System Monitor and Recorder

One of the projects I worked on at ARA was in debugging and improving a subsystem that collects sensor data to create recordings and a live system report to give external operators a better idea of the vehicle state, as part of a larger team I helped support.  I worked specifically in implementing failsafes to help with malfunctioning or inaccessible sensor data, as well as integrating a machine learning script into our dockerized ROS environment, modifying it to run on live audio instead of pre-recorded files. 

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

### Graduate Internship--RightHand Robotics: Steerable-Mirror Camera Integration

During my Ph.D, I interned with RightHand Robotics, a company working on pick-and-place logistics automation systems.  While there, I worked on integrating a steerable-mirror camera into their existing state machine, using the camera to track the robot's end-effector and scan barcodes in motion.  This involved slight modifications to the existing arm's path to ensure maximum chance of barcode visibility.  It also involved quite a bit of integration work, to dynamically change mirror positions from outside of the camera's specialized software, which had OS and other requirements incompatiple with integration into the robot's state machine.


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
