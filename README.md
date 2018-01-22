# CarND-Controls-MPC
Self-Driving Car Engineer Nanodegree Program

My solution is contained in these files: [main](src/main.cpp) [MPC](src/MPC.cpp)

My code is calculating tracking points in order to steer the udacity simulated car to drive in the correct direction.

---

## The Model
Student describes their model in detail. This includes the state, actuators and update equations.

## Timestep Length and Elapsed Duration (N & dt)
Student discusses the reasoning behind the chosen N (timestep length) and dt (elapsed duration between timesteps) values. Additionally the student details the previous values tried.

## Polynomial Fitting and MPC Preprocessing
A polynomial is fitted to waypoints.

If the student preprocesses waypoints, the vehicle state, and/or actuators prior to the MPC procedure it is described.

## Model Predictive Control with Latency
Implemented a Model Predictive Control handling a 100 millisecond latency. 
TODO Student provides details on how they deal with latency.

## Simulation
Vehicle successfully drives a lap around the track, and no tire left the drivable portion of the track surface.