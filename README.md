# robot_position_3d

This is the ROS plugin for knowing the position of the model on gazebo

Steps to use this plugin:

1. Clone common_msgs for melodic and compile it using the command
```
catkin_make --only-pkg-with-deps common_msgs
```
2. `source devel/setup.bash`
3. Compile the robot_position_plugin package using the command,
```
catkin_make --only-pkg-with-deps robot_position_plugin
```
4. `source devel/setup.bash`
5. Launch the launch file using the command,
```
roslaunch robot_position_plugin launch_3d_position.launch
```
6. After Step 5, we can see gazebo is up with the box model
7. We can see the position of the model published on `/model_1/link_1/pose`
8. To see the floor number, check on topic `/elevator`
