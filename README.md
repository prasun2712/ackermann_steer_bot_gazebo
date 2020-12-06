# ackermann_steer_bot_gazebo
This repository contains ackermann-steer robot gazebo (tricycle model). This is done as a fun project and work is still going on.

## Dependencies
* [ROS Noetic](http://wiki.ros.org/noetic) - Installation instructions [here](http://wiki.ros.org/noetic/Installation/Ubuntu) for ubuntu.
* Create [catkin workspace](http://wiki.ros.org/catkin/Tutorials/create_a_workspace).
* Install [Ackermann Steering Controller](http://wiki.ros.org/ackermann_steering_controller).

## Place the package in your catkin_ws and launch
```
cd <to_catkin_ws>/src
git clone https://github.com/prasun2712/ackermann_steer_bot_gazebo.git
rospack profile
roslaunch ackermann_steer_bot_gazebo ackermann_steer_empty_world.launch
```
**Open rqt_gui**
```
rosrun rqt_gui rqt_gui
```
Go to **Plugins->Robot Tools->Robot Steering**. In topic put : ***/mobile_base_controller/cmd_vel***

## Video
**Click the image below to see the demo video for basic movement of robot using ROS command velocity.**
[![Demo Video.](https://github.com/prasun2712/ackermann_steer_bot_gazebo/blob/main/pictures/ackermann_steer_bot.png)](https://youtu.be/z7iN2RVpc_0)

## ToDo
* Make it a bot equipped with multiple sensors (2D/3D lidar, IMU, RGBD camera, etc).
* Packages to perform localization, mapping(2D/3D) and navigation.
* Details will be updated in the same repo, stay tuned.