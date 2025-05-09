---
title: "Flight Dynamics and Controls"
layout: single-portfolio
excerpt: "Modeling, simulation, control, estimation, and path planning for a fixed wing UAV. The final result of the project is a simulator built from scratch with implementations of IMU, pressure, and GPS sensors, Extended Kalman Filter and RRT path planning. <br/><br/><img src='/images/flightdynamics.png' width='500'>"
collection: projects
---

This project was a semester long project for Dr. Tim McLain's course on Flight Dynamics and Controls. The [code](https://github.com/curtiscjohnson/flight_dynamics) is available on Github.

The project was broken into multiple parts:

## Part 1: Modeling and Simulation
This section tests out control surface simulation by setting various elevator, throttle, rudder, or aileron commands. It doesn't have trim calculated yet, so flight is unstable. It also checks the dynamics simulation of the fixed wing UAV by simply applying forces in different directions and observing the flight path.

<iframe width="560" height="315" src="https://www.youtube.com/embed/O0wbCJOqsWw?si=Ivm5lW5bXAdpeOY9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Part 2: Heading and Altitude Control
Low level controllers are working! Data plots on the right show commanded heading and altitudes (and corresponding state trajectories) while the left simulates the flight of the UAV.

<iframe width="560" height="315" src="https://www.youtube.com/embed/PZ5ADEJKhXc?si=a8IkuZAHIYo9SBF0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Part 3: Sensor Modeling and Fusion
This simulates the flight of the UAV now using sensor data (as opposed to true state data). The sensor data is corrupted with noise (red lines on the plots) and the states are estimated with an EKF. I added IMU, pressure, and GPS sensor models to the simulation. On the right is the sensory output and on the left are the 'true' state trajectories and commands.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4shBKClj2xA?si=pCQwYk59cG6iAgWh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Part 4: Path Planning and Following
This video demonstrates various types of path following capabilities (e.g. lines and orbits). We describe the longitudinal and lateral tracking problems in terms of a vector field that converges to the desired path. This video shows a path planner result through a 'city' of obstacles. The path planner uses Voronoi graphs or an RRT with smoothing to calculate the final displayed trajectory.

<iframe width="560" height="315" src="https://www.youtube.com/embed/2m-Wyjf5mmA?si=0tWu7tOWuOJpwy3P" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>




