---
title: "MoCap project: MiCap"
excerpt: "A DIY inertial motion capture system to explore affordable, accessible solutions for real-time character animation."
header:
    video:
        id:
        provider: youtube
    teaser: assets/images/work-in-progress.png

sidebar:
  - title: "Role"
    text: "Sole Developer"
  - title: "Responsibilities"
    text: "Project Research, Network Engineering, Rigging, Hardware design and assembly"
  - title: "Tools Used"
    text: "Unity, C++, Arduino, ESP32, UDP Sockets"
gallery:
  - url: assets/images/3D.png
    image_path: assets/images/3D.png
  - url: assets/images/PCB Design.png
    image_path: assets/images/PCB Design.png
  - url: assets/images/Schematic design.png
    image_path: assets/images/Schematic design.png
  - url: assets/images/Technical Drawing.png
    image_path: assets/images/Technical Drawing.png
gallery2:
  - url: assets/images/3D.png
    image_path: assets/images/3D.png
  - url: assets/images/PCB Design.png
    image_path: assets/images/PCB Design.png
  - url: assets/images/Schematic design.png
    image_path: assets/images/Schematic design.png
  - url: assets/images/Technical Drawing.png
    image_path: assets/images/Technical Drawing.png
---

I am developing a DIY inertial motion capture system to explore affordable, accessible solutions for real-time character animation. 
The project combines embedded hardware, networking, and animation pipelines to stream body motion into Unreal Engine. While still in progress, it demonstrates my ability to design complex systems, solve integration challenges, and iterate on technical workflows.

## My Role & Responsibilities

* Designed modular sensor units using ESP microcontrollers, BNO085 IMUs, and LiPo batteries.

* Designed and Soldered Custom PCBs and Cases to create a simpler and more modular design.

* Implemented a UDP networking pipeline in C++ for reliable real-time data transfer to a PC.

* Developed threaded server architecture to handle multiple data streams simultaneously.

* Created a prototype animation rig in Unity to test motion playback and calibration.


## Achievements So Far

* Sensor prototypes successfully transmit rotation data wirelessly.

* UDP client/server runs with low latency and supports multiple IMU streams.

* Proof-of-concept rig integration in Unity.

<div style="max-width: 50%">
    {% include gallery id = "gallery"  caption="PCB, schematics, technical drawings" %}
</div>

## Next Steps

* Expand from 2–3 sensors to a full-body tracking system.

* Build a calibration workflow for accuracy and ease of use.

* Add debugging & visualization tools for live sensor data.

Explore accessibility applications, such as alternative interfaces for creators or performers who may not have access to expensive mocap systems.

## Skills Demonstrated

* Programming & Systems Design – UDP networking, threading, real-time data handling.

* Hardware Integration – ESP microcontrollers, IMUs, custom power management.

* Animation Pipelines – Rigging & data playback in Unreal.

* Problem-Solving & Iteration – Debugging latency, packet loss, and synchronization issues.

## Reflection

This project highlights my ability to work at the intersection of hardware, software, and interactive media. 
Beyond its technical scope, 
I am interested in how low-cost mocap can expand access to creative tools, for more inclusive and socially impactful goals.