---
title: "MuJoCo Simulation of Continuum Robots"
layout: single-portfolio
excerpt: "A novel way to simulate soft continuum robots in MuJoCo. <br/><br/><img src='/images/baloo_mujoco.png' width='700'>"
collection: projects
---

[MuJoCo](https://mujoco.readthedocs.io/en/latest/overview.html) is a well-known physics engine that is used to simulate robotic systems. However, it is not designed to simulate soft continuum robots. I developed a novel way to simulate soft continuum robots in MuJoCo by using a series of rigid bodies connected by joints. This method allows for the simulation of soft continuum robots in MuJoCo.

We've used it to simulate highly dynamic tasks like throwing

![Baloo MuJoCo Simulation](/images/mujoco_throw_open.png)

I'm currently using it to train a reinforcement learning policy to control Baloo to manipulate large objects:

<iframe width="560" height="315" src="https://www.youtube.com/embed/v0C7hRXVU30?si=Dg46qfhA8cfRsJQ4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>



