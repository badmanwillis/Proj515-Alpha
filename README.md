# Proj515-Alpha

Part of the navigation stack for the Alpha robot. This repo contains a ros package alpha_urdf, which features a urdf model of the robot, as well as intergrated lidar (rplidar a1) and odometry (custom magnetic encoders based on the AS5600 chip).

## Getting Started

You will need:

* Ubuntu 16.04
* ros kinetic
* rplidar A1
* (AS5600)[https://ams.com/as5600]

### Installing alpha_urdf

Copy the alpha_urdf package into your_workspace/src directory. Then rebuild the workspace.

```
catkin_make
```

### Installing the rplidar package

You will also need the rplidar package in the your_workspace/src directory

https://github.com/Slamtec/rplidar_ros
