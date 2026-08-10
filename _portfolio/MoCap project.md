---
title: "IMU Motion Tracker: MiCap"
excerpt: "A DIY inertial motion capture system to explore affordable, accessible solutions for real-time character animation."
header:
    video:
      id: 3nuybgIpUBY
      provider: youtube
    teaser: assets/images/MiCapFrontPage.png
sidebar:
  - title: "Role"
    text: "Developer"
  - title: "Responsibilities"
    text: "Research, Network engineering, Rigging, Programming, Debugging, Modelling, Soldering, Embedded Systems, ML"
  - title: "Tools Used"
    text: "Unity, Unreal, C++, Arduino, ESP32, UDP Protocol, Fusion 360, KiCad, Edge Impulse"
video2:
  id: V9PdawP01Ko
  provider: youtube
  teaser: assets/images/MiCapFrontPage.png
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
gallery3:
  - url: assets/images/NN_Shape.png
    image_path: assets/images/NN_Shape.png
  - url: assets/images/Impulse Design.png
    image_path: assets/images/Impulse Design.png

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


## Current Progress : Motion Classification Experiment

I am currently experimenting with the benefits of using an ML Based Classification Model with the technology.
As seen in the video above, I am using the modules to control the game punchout! Wii, but I struggled with getting the parameters to fit perfectly in each situation. Due to this constraint I began experimenting with the idea of using an ML based classification model.

### Data Collection

I began by collecting the data and using Edge Impulse's CLI Data Forwader, then, I was able to visualize the data and consider what the best data for the task would be. I decided on gyro, Accel and Linear Accel, as this would be sufficient for differentiating what actions were being made.

I decided to collect three movement classes:

* Idle
* Hit
* Block


I have trained and deployed a preliminary inference model, but the data I performed the testing on was about 2 milliseconds long, which is too long for this use case.


### Data Pre-Processing

While Data Pre-Processing is a difficult task for embedded ML, Using Edge Impulse's Spectral Analysis block allows the Model to be able to train on repetitive motion, using F.F.T(Fast Fourier Transformation). It essentiallly takes a window of the raw data and splits it into features, which can be used as input for the Neural Network.


### Model Design

The Neural Network is composed of 53 input neurons, 2 hidden layers with 20 and 10 neurons each and an output of 3, those being our possible movements.


### Training and Testing

After generating the features(our input parameters from the raw data), I trained and the model performed with 100% accuracy! This pleasantly surprised me, as it was my first time training an NN. But the testing proved more challenging. Once Tested I received consistent confusion with a particular block data. I assumed that this must be an error and replaceed it, then receiving 100%, but when live training, I noticed this error pattern continued.

After further investigation, I discovered I had written the reports for my IMU in a way that caused it to return the same data accross all three reports(Gyro, Accel, LAccel) After fixing this, I was able to train and test with 100% accuracy, as well as during live deployment.

{% include gallery id = "gallery3" layout = "full" caption="Images of the NN's structure, Results and Impulse Training Block" %}
{% include video id = "video2" layout = "full" caption="A video of the original functionality" %}


## Reflection

This project highlights my ability to work at the intersection of hardware, software, and interactive media. 

Beyond its technical scope, I am interested in how low-cost mocap can expand access to creative tools, allowing for people to gain the opportunity to use powerful tech with a lower barrier of entry.



<!---
 -->