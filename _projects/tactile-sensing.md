---
title: "Large Area Tactile Sensing"
layout: single-portfolio
excerpt: "A sensor I developed to give robots a sense of touch over their entire structure. <br/><br/><img src='/images/tactile_sensor_block_diagram.png' width='700'>"
collection: projects
---


Robotic manipulation research aims to enhance robot capabilities in unstructured environments, where objects vary greatly. Tactile sensing plays a crucial role, as cameras often struggle with occlusion or delicate handling tasks. While additional cameras can address occlusion, this approach does not scale well for open-world manipulation. Tactile sensors, akin to human touch, provide critical information that vision cannot capture.

Typically, tactile sensors are exclusively located at the robot’s end effector, offering high-resolution measurements over small areas. 

Our work introduces a novel large-area tactile sensing solution designed for whole-arm manipulation. This approach extends sensing capabilities beyond the end effector, enabling robots to handle unpredictable contact patterns across broad surfaces.

<img src="/images/hand_tactile_plot.png" height="400">


The sensor works by measuring the resistance between a conductive layer and a grid of electrodes. When an object contacts the sensor, the resistance changes, providing information about the contact location and pressure.

<img src="/images/tactile_sensor_block_diagram.png" height="400">

These sensors can be mounted on a robots structure and help with tasks that might be difficult without a sense of touch, like lifting large and awkward objects. Here's a photo of an early prototype sensor on Baloo while lifting a kayak:



<p float="left">
  <img src="/images/baloo-kayak-tactile.png" height="400" />
  <img src="/images/kayak-tactile-output.png" height="400" /> 
</p>