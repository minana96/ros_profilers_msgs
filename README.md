# *ros_profilers_msgs* ROS package

This repository represents the *ros_profilers_msgs* ROS pacakge, the package that contains service definitions for power consumption, CPU usage and RAM urilisation measurement collecion. The *ros_profilers_msgs* package is intended for ROS Melodic. The repository needs to be cloned to the catkin workspace on both the robot and the PC (for ROS nodes that provide services for measurement collection and Robot Runner, which initiates the service calls, respetfully) and compiled with following commands:
```bash
cd <catkin_ws_dir>/src
git clone git@github.com:minana96/ros_profilers_msgs.git
cd ..
catkin_make
```
## Package content

The package consists of one directory, *srv*.

### srv

The directory contains four service definitions:
- **StartPowerMeasurements.srv**: service for initiation of power consumption measurement collection;
- **StopPowerMeasurements.srv**: service for termination of power consumption measurement collection, which returns the obtained measurement results;
- **StartResourceMeasurments.srv**: service for initiation of CPU usage and RAM utilisation measurement collection;
- **StopResourceMeasurments.srv**: service for termination of CPU usage and RAM utilisation measurement collection, which returns the obtained measurement results.
