# rtabmap-turtlebot3
This is a simple tutorial for those who need to practice with ROS and Gazebo simulator. Also you can learn a little about SLAM and [RTAB-Map](http://introlab.github.io/rtabmap/) algorithims.<br />
Here is the Youtube Link.(Coming Soon)

<img src="https://github.com/kavehsgh/rtabmap-turtlebot3/blob/main/Pictures/Screenshot%20(200).png">


### Dependencies

ROS version: Noetic<br />
OS: Ubuntu 20.4<br />
Gazebo Version: 11

I am assuming that you did install [ROS](http://wiki.ros.org/noetic/Installation) and [Gazebo](https://classic.gazebosim.org/).

## Step 1 - installing required packages

First we start from installing some ros packages.
```
sudo apt-get install ros-kinetic-joy ros-kinetic-teleop-twist-joy \
  ros-kinetic-teleop-twist-keyboard ros-kinetic-laser-proc \
  ros-kinetic-rgbd-launch ros-kinetic-depthimage-to-laserscan \
  ros-kinetic-rosserial-arduino ros-kinetic-rosserial-python \
  ros-kinetic-rosserial-server ros-kinetic-rosserial-client \
  ros-kinetic-rosserial-msgs ros-kinetic-amcl ros-kinetic-map-server \
  ros-kinetic-move-base ros-kinetic-urdf ros-kinetic-xacro \
  ros-kinetic-compressed-image-transport ros-kinetic-rqt* \
  ros-kinetic-gmapping ros-kinetic-navigation ros-kinetic-interactive-markers
```


