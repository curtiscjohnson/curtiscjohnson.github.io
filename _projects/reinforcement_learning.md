---
title: "Reinforcement Learning for Whole Body Manipulation"
layout: single-portfolio
excerpt: " <br/><br/><img src='/images/baloo_rl.png' width='700'>"
collection: projects
---

Building on top of the MuJoCo simulation I've built, I'm working on training Baloo to manipulate large objects:

<iframe width="560" height="315" src="https://www.youtube.com/embed/v0C7hRXVU30?si=Dg46qfhA8cfRsJQ4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Each object has a random size and mass and the objective is to lift the object off the floor successfully. I'm using the implementation of PPO from the [Stable Baselines3](https://stable-baselines3.readthedocs.io/en/master/) library. 

For this project, I'm focused on a few different aspects:
- **Reward shaping**: The reward function is crucial for training the robot to perform the task. I'm experimenting with different reward functions to see which one works best.
- **Imitation learning**: I'm exploring how an expert trajectory can help accelerate learning.
- **Sim2real**: I'm working on transferring the learned policy to the real robot. This is a challenging problem, but I've put in lots of effort to maximize the realism of the MuJoCo simulation.
- **Tactile Sensing**: I'm exploring the effects of whole-body tactile sensing on the learning process.