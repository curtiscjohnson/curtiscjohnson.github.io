---
title:  "PneuDrive: An Embedded Pressure Control System and Modeling Toolkit for Large-Scale Soft Robots"
collection: publications
permalink: /publication/2023-pneudrive
date: 2023-11-1
venue: '2024 7th International Conference on Soft Robotics (RoboSoft)'
paperurl: '/files/pneudrive.pdf'
link: 'https://ieeexplore.ieee.org/abstract/document/10521958'
authors: CC Johnson, DG Cheney, DL Cordon, MD Killpack
teaser: /images/DaisyChainDiagram.png
abstract: "In this paper, we present a modular pressure control system called PneuDrive that can be used for large-scale, pneumatically-actuated soft robots. The design is particularly suited for situations which require distributed pressure control and high flow rates. Up to 4 embedded pressure control modules can be daisy-chained together as peripherals on a robust RS-485 bus, enabling closed-loop control of up to 16 valves with pressures ranging from 0-100 psig (0-689 kPa) over distances of more than 10 meters. The system is configured as a C++ ROS node by default. However, independent of ROS, we provide a Python interface with a scripting API for added flexibility. We demonstrate our implementation of PneuDrive through various trajectory tracking experiments for a three-joint, continuum soft robot with 12 different pressure inputs. Finally, we present a modeling toolkit with implementations of three dynamic actuation models, all suitable for real-time simulation and control. We demonstrate the use of this toolkit in customizing each model with real-world data and evaluating the performance of each model. The results serve as a reference guide for choosing between several actuation models in a principled manner."
---




