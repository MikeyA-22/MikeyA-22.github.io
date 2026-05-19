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
    text: "Research, Network engineering, Rigging, Programming, Debugging, Modelling, Soldering, Embedded Systems"
  - title: "Tools Used"
    text: "Unity, Unreal, C++, Arduino, ESP32, UDP Protocol, Fusion 360, KiCad"
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
  - url: assets/images/startingpoint.png
    image_path: assets/images/startingpoint.png
  - url: assets/images/mocapmodulepics.png
    image_path: assets/images/mocapmodulepics.png
---

I am developing a DIY inertial motion capture system to explore affordable, accessible solutions for real-time character animation. 
The project combines embedded hardware, networking, and animation pipelines to stream body motion into Unity Engine.

## My Role & Responsibilities

* Designed modular sensor units using ESP32 microcontrollers, BNO085 IMUs(Inertial Measurement Units), and LiPo batteries.

* Implemented a UDP networking pipeline in C++ for reliable real-time data transfer to a PC.

* Developed threaded server architecture to handle multiple data streams simultaneously.

* Created a prototype animation rig in Unity to test motion playback and calibration.

<div style="max-width: 50%">
    {% include gallery id = "gallery"  caption="PCB, schematics, technical drawings" %}
</div>

## Achievements So Far

* Sensor prototypes successfully transmit rotation data wirelessly.

* UDP client/server runs with low latency and supports multiple IMU streams.

* Proof-of-concept rig integration in Unity Engine.


{% include gallery id = "gallery2" layout = "full" caption="First Iteration and Current Iteration" %}

## Next Steps

* Expand from 2–3 sensors to a full-body tracking system.

* Build a calibration workflow for accuracy and ease of use.

* Add debugging & visualization tools for live sensor data.

Explore accessibility applications, such as alternative interfaces for creators or performers who may not have access to expensive mocap systems.

## Skills Demonstrated

* Programming & Systems Design – UDP networking, threading, real-time data handling.

* Hardware Integration – ESP microcontrollers, IMUs, custom power management.

* Animation Pipelines – Rigging & data playback in Unity.

* Problem-Solving & Iteration – Debugging latency, packet loss, and synchronization issues.

## Reflection

This project highlights my ability to work at the intersection of hardware, software, and interactive media. Beyond its technical scope, I am interested in how low-cost mocap can expand access to creative tools, allowing for people to gain the opportunity to use powerful tech with a lower barrier of entry.