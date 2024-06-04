---
title: "Simultaneous Localization and Mapping (SLAM)"
layout: single-portfolio
excerpt: "Various implementations of localization and mapping algorithms.  <br/><br/><img src='/images/slam-demo.gif' width='500'>"
collection: projects
---

This project was a semester long project for Dr. Joshua Mangelson's course on SLAM. The [code](https://bitbucket.org/cjohns94/workspace/projects/SLAM) is available on Bitbucket.


## Occupancy Grid Mapping 
To generate the data used in this lab, we simulated a robot with 20 laser range finders spread out at various angles.

Each of these laser range finders is directed in a slightly different direction on the front of the robot. We then navigated the robot through a simulated building, entering each room one-by-one.

![real](/images/real-building.png "real building")

At each time step we recorded the current “ground-truth” pose of the robot as well as the range returned by
each of the 20 laser range finders when the robot was at the recorded pose.

To accomplish the mapping, I implemented a laser range finder model that updates each cell with the log-odds of the cell being occupied. The log-odds are updated based on the inverse sensor model and the range data from the laser range finder. The inverse sensor model is a function that takes in the range data and the pose of the robot and returns the probability of the cell being occupied given the range data. The log-odds are then updated based on the probability of the cell being occupied.


Here are my results:
![grid](/images/occupancy-grid-mapping.png "occupany grid")

## Part 2: EKF/UKF Landmark Based Localization
I implemented both an EKF and UKF in order to localize the robot using odometry measurements and bearing-only measurements to landmark features. 

The setting was in a robot soccer arena with individially landmarks with unique IDs.

![soccer](/images/robot-localization-soccer.png "soccer")

And here are my results with the robot driving around the soccer field. 

EKF:
![ekf](/images/video_efk.gif "ekf")


UKF:
![ukf](/images/video_ukf.gif "ukf")




