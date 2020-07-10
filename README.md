# Turtlebot3-Localization-and-Mapping-SLAM
Creating Indoor map with Stimultneous Localization and Mapping (SLAM) and Gmapping with turtlebot3.

....

First, install turtlebot3 simulation packages.


Then, run the following commands:

// launch gazebo world with a turtlebot.

$ roslaunch turtlebot3_gazebo turtlebot3_world.launch 

....

// launch SLAM with rviz and spacify gmapping method.

$ roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping

....

// launch key teleop to cover the whole area. 

$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch 

....

// when you finish, save the map using map_server package.

$ rosrun map_server map_saver -f ~/map
