# Leg Detector
This is ROS package that implements a leg detector from a LaserScan message, and publish the position of humans in a PoseArray message and markers to visualize the position of human in rviz.

This code is based on the work described in:

Bellotto, N.; Huosheng Hu, "Multisensor-Based Human Detection and Tracking for Mobile Service Robots," Systems, Man, and Cybernetics, Part B: Cybernetics, IEEE Transactions on , vol.39, no.1, pp.167,181, Feb. 2009
doi: 10.1109/TSMCB.2008.2004050

Run this package by typing 

```
roslaunch edge_leg_detector edge_leg_detector.launch laser_scan:=
```

Where ```[LASER_SCAN_TOPIC]``` is the name of the topic with the LaserScan sensor data. For example, if the name of the topic is ```/scan``` then, the leg detector can be initialized as: 

```
roslaunch edge_leg_detector edge_leg_detector.launch laser_scan:=/base_scan
```
