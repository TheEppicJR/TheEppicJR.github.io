---
layout: post
title:  "Virtual Linkage Arm"
date:   2024-02-26 23:26:53 -0800
categories: jekyll update
---

<img src="/assets/virtual_linkage/vl_16.jpeg" width = 400 class="rounded-image">
<br>
This is the arm I designed for the 2018 FIRST Robotics Competition with a rather novel design. In order to have a single actuator (in reality two motors running in parallel, but still one logical axis) operate a two joint arm with the output axis follow a vertical linear path. Additionally a second rotary axis about the output axis of the first linkage is driven from the base of the arm through a series of pullies such that there is no angle correction needed. Aside from the chain drive at the base used for mechanical advantage there is no backlash in the system as it is driven through spliced kevlar lines.
<br>
<br>
<img src="/assets/virtual_linkage/vl_21.jpeg" width = 600 class="rounded-image">
<br>
In order to get wrist axis on the end of the forearm to track vertically, the forearm needs to have the opposite angle with respect to the robot as the arm (I am using arm to describe specifically the upper arm, as it is both technically correct academic jargon and in our case the forearm is above the upper arm). To do this we connect the forearm to the shoulder (our datum) with a 1:2 ratio, which results in the wrist tracking vertically. Here is a gif of a lego proof of concept:
<br>
<br>
<img src="/assets/virtual_linkage/vl_31.gif" width = 400 class="rounded-image">
<br>
The ratio used in the proof of concept isn't exactly 1:2 so it does not follow a perfectly vertical path, but it is close enough to demonstrate the concept.
<br>
Then there is the pulley system to actuate the wrist, which consists of two 1:1 stages driven by another planetary mounted in the shoulder which drives the first pulley via a chain.
<br>
<br>
<img src="/assets/virtual_linkage/vl_26.jpeg" width = 400 class="rounded-image">
<br>
And then both planetares, the fixed pulley, wrist pulley, bearings, and arm drive sprocket are all densely, although not exactingly serviceably, packaged together using a 1"x3" and 1"x2.5" aluminum box tubing.
<br>
<br>
<img src="/assets/virtual_linkage/vl_24.jpeg" width = 400 class="rounded-image">
<br>
Aside from serviceability, this arm had two main issues: first was that the torque required to lift the arm was hugely non-linear which the software team was not able to deal with sufficiently in the time available, although this was mitigated with springs. The second issue was that the Versa Planetary gearboxes that were used were fraught with design flaws, all of which were observed: sun gears not sufficiently attached to the spline driving them (this failure only appears near max torque), shattered planet carriers, and binding issues with the encoders. 
<br>
<br>
<img src="/assets/virtual_linkage/vl_29.jpeg" width = 400 class="rounded-image">
<br>
But overall it was a good year, I learned a lot of the most fundamental principles of mechanical design during this project, and it turned out alright.
<br>
<br>
<img src="/assets/virtual_linkage/vl_30.webp" width = 600 class="rounded-image">