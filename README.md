# Proj515-Alpha

Part of the navigation stack for the Alpha robot. This repo contains a ros package alpha_urdf, which features a urdf model of the robot, as well as intergrated lidar (rplidar a1) and odometry (custom magnetic encoders based on the AS5600 chip).

## Getting Started

You will need:

* Ubuntu 16.04
* ros kinetic
* [rplidar A1](http://wiki.ros.org/rplidar)
* [AS5600](https://ams.com/as5600) magnetic encoders

### Installing alpha_urdf package

Copy the alpha_urdf package into your_workspace/src directory. Then rebuild the workspace.

```
catkin_make
```

### Installing the rplidar package

You will also need the rplidar package in the your_workspace/src directory

https://github.com/Slamtec/rplidar_ros

This will require you to rebuild the workspace.

## Deployment

From the root directory of your workspace.

Source your workspace
```
source devel/setup.bash 
```

Run the launch file. Rviz should start, and display the robot.
```
roslaunch alpha_urdf display.launch

```

In Rviz:
* change the fixed frame to "odom"
* add a new display "LaserScan". Set the topic to /scan


You should now be able to view the robot model in rviz, along with the odometry and lidar data.

# todo
* package not whole repo
* rename paths in files alpha.xml, and display.launch

