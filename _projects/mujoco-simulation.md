---
title: "MuJoCo Simulation of Continuum Robots"
layout: single-portfolio
excerpt: "A novel way to simulate soft continuum robots in MuJoCo. <br/><br/><img src='/images/baloo_mujoco.png' width='700'>"
collection: projects
---

[MuJoCo](https://mujoco.readthedocs.io/en/latest/overview.html) is a well-known physics engine that is used to simulate robotic systems. However, it is not designed to simulate soft continuum robots. I developed a novel way to simulate soft continuum robots in MuJoCo by using a series of rigid bodies connected by joints. This method allows for the simulation of soft continuum robots in MuJoCo.

We've used it to simulate highly dynamic tasks like throwing.

![Baloo MuJoCo Simulation](/images/mujoco_throw_open.png)

Currently, I'm using it to simulate Baloo, a soft robotic torso that I'm building for my PhD work. The simulation is used to develop control and planning algorithms for whole body manipulation.

![Baloo MuJoCo Simulation](/images/baloo_mujoco.png)


