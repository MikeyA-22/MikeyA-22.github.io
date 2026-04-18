---
title: "IMU Motion Tracker: MiCap"
excerpt: "A DIY inertial motion capture system to explore affordable, accessible solutions for real-time character animation."
header:
    video:
        id: V9PdawP01Ko
        provider: youtube
    teaser: assets/images/MiCapFrontPage.png

sidebar:
  - title: "Role"
    text: "Developer"
  - title: "Responsibilities"
    text: "Project Research, Network engineering, Rigging, Hardware design and assembly, Embedded Systems"
  - title: "Tools Used"
    text: "Unity, C++, Arduino, ESP32, UDP Protocol"
---

I am developing a DIY inertial motion capture system to explore affordable, accessible solutions for real-time character animation. 
The project combines embedded hardware, networking, and animation pipelines to stream body motion into Unity Engine.

# My Role & Responsibilities

* Designed modular sensor units using ESP32 microcontrollers, BNO085 IMUs(Inertial Measurement Units), and LiPo batteries.

* Implemented a UDP networking pipeline in C++ for reliable real-time data transfer to a PC.

* Developed threaded server architecture to handle multiple data streams simultaneously.

* Created a prototype animation rig in Unity to test motion playback and calibration.


# Achievements So Far

* Sensor prototypes successfully transmit rotation data wirelessly.

* UDP client/server runs with low latency and supports multiple IMU streams.

* Proof-of-concept rig integration in Unity Engine.


<figure class="align-right">
<img src="{{ site.url }}{{ site.baseurl }}assets/images/mocapmodulepics.jpg" alt="">
  <figcaption>Current State of the Modules</figcaption>
</figure>

# Next Steps

* Expand from 2–3 sensors to a full-body tracking system.

* Build a calibration workflow for accuracy and ease of use.

* Add debugging & visualization tools for live sensor data.

Explore accessibility applications, such as alternative interfaces for creators or performers who may not have access to expensive mocap systems.

# Skills Demonstrated

* Programming & Systems Design – UDP networking, threading, real-time data handling.

* Hardware Integration – ESP microcontrollers, IMUs, custom power management.

* Animation Pipelines – Rigging & data playback in Unity.

* Problem-Solving & Iteration – Debugging latency, packet loss, and synchronization issues.

## Reflection

This project highlights my ability to work at the intersection of hardware, software, and interactive media. Beyond its technical scope, I am interested in how low-cost mocap can expand access to creative tools, allowing for people to gain the opportunity to use powerful tech with a lower barrier of entry.