# Leg Detector
This is ROS package that implements a leg detector from a LaserScan message, and publish the position of humans in a PoseArray message and markers to visualize the position of human in rviz.

This code is based on the work described in:

Bellotto, N.; Huosheng Hu, "Multisensor-Based Human Detection and Tracking for Mobile Service Robots," Systems, Man, and Cybernetics, Part B: Cybernetics, IEEE Transactions on , vol.39, no.1, pp.167,181, Feb. 2009
doi: 10.1109/TSMCB.2008.2004050

Run this package by typing 

```
roslaunch edge_leg_detector edge_leg_detector.launch laser_scan:=/base_scan
```
Open another terminal and run the following command:
```
rosrun rviz rviz
```
In the rviz window, make Fixed Frame as base_laser_link
Add LaserScan topic "base_scan"
Add Marker topic "marker2"

