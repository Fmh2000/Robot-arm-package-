HOW-TO-INSTALL-ROS-KINETIC
===============


The below commands are for installing robot arm packageon Ubuntu 16.04:

Add ardunio-robot-arm package to src folder
-----
```shell 


cd ~/catkin_ws/src
sudo apt install git

git clone https://github.com/smart-methods/arduino_robot_arm.git 

```

Install all dependcies
-----

```shell 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y
 

sudo apt-get install ros-kinetic-moveit

 
sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui

sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control

```
Compile the package 
-----
```shell 
roslaunch robot_arm_pkg check_motors.launch

```
Output
-----

