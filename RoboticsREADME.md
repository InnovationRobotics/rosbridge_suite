Thw version that works with our setup:
1. ROS # with Unity3d running on Windows 10
2. Bridge to the agent on Ubuntu 18.04 supporting ROS Melodic.

Note that I tried the version 0.9.0 and it already was not registering clients to topics of the ROS network.

In order to use this version, do:
1. Create catkin_ws: mkdir -p ~/catkin_ws/src; cd ~catkin; catkin_make 
2. Clone this repository to catkin_ws/src; checkout branch smartload;
3. Build the project: catkin_make
4. Source ~/catkin_ws/devel/setup.bash

In order to run: 
roslaunch rosbridge_server rosbridge_websocket.launch
