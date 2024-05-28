# rtabmap-turtlebot3
This is a simple tutorial for those who need to practice with ROS and Gazebo simulator. Also you can learn a little about SLAM and [RTAB-Map](http://introlab.github.io/rtabmap/) algorithims.<br />
Here is the Youtube Link. (https://youtu.be/beUP-1fil3c?si=A3cLRneqDPDw_gAM)

<img src="https://github.com/kavehsgh/rtabmap-turtlebot3/blob/main/Pictures/Screenshot%20(200).png">


### Dependencies

ROS version: Noetic<br />
OS: Ubuntu 20.4<br />
Gazebo Version: 11

I am assuming that you did install [ROS](http://wiki.ros.org/noetic/Installation) and [Gazebo](https://classic.gazebosim.org/).

## Step 1 - installing required packages

First we start from installing some ros packages.
```
sudo apt-get install ros-noetic-joy ros-noetic-teleop-twist-joy \
  ros-noetic-teleop-twist-keyboard ros-noetic-laser-proc \
  ros-noetic-rgbd-launch ros-noetic-depthimage-to-laserscan \
  ros-noetic-rosserial-arduino ros-noetic-rosserial-python \
  ros-noetic-rosserial-server ros-noetic-rosserial-client \
  ros-noetic-rosserial-msgs ros-noetic-amcl ros-noetic-map-server \
  ros-noetic-move-base ros-noetic-urdf ros-noetic-xacro \
  ros-noetic-compressed-image-transport ros-noetic-rqt* \
  ros-noetic-gmapping ros-noetic-navigation ros-noetic-interactive-markers
```

## Step 2 - installing Turtlebot3 related packages

```
sudo apt install ros-noetic-turtlebot3-simulations ros-noetic-turtlebot3-navigation ros-noetic-dwa-local-planner
```

## Step 2 - Launch the simulation

```
export TURTLEBOT3_MODEL=waffle
roslaunch turtlebot3_gazebo turtlebot3_house.launch
```
In another terminal tab:
```
export TURTLEBOT3_MODEL=waffle
roslaunch rtabmap_ros demo_turtlebot3_navigation.launch
```

