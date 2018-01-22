# CarND-Controls-MPC
Self-Driving Car Engineer Nanodegree Program

My solution is contained in these files: [main](src/main.cpp) [MPC](src/MPC.cpp)

My code is calculating tracking points in order to steer the udacity simulated car to drive on the track.

---
## The Model
Used the following constraints based on the following vehicle model:
![Vehicle Model](Model.png)

## Polynomial Fitting and MPC Preprocessing
Moved and rotated the vehicle points, to align with the regular x-y coordinates, in order to make it easier to understand.

## Timestep Length and Elapsed Duration (N & dt)
I chose N (timestep length) = 10 and and dt (elapsed duration between timesteps) as 0.1, in order to get 10 values totalling a one second.

## Model Predictive Control with Latency
Implemented a Model Predictive Control handling a 100 millisecond latency.

As was sugessted in one of the lectures by udacity TAs, the way to handle latency is to delay initializing the delta and acceleration constraints by one time period, i.e.
      `AD<double> delta0 = vars[delta_start + t - 2];
      AD<double> a0 = vars[a_start + t - 2];`

## Simulation
I am unable to install the Ipopt libraries on my mac, but will look for an alternate machine and re-run it soon.