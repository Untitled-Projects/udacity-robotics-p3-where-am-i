Udacity Robotics Software Engineer Nanodegree Project 3 Where am I by Michael Strobl


Start the project

0- Add Teleop Twist Keyboard 

    $ cd ~/catkin_ws/src
    $ git clone https://github.com/ros-teleop/teleop_twist_keyboard

1- Build the project:
    
    $ cd ~/catkin_ws
    $ catkin_make


2- Launch the robot inside your world

    $ cd ~/catkin_ws
    $ source devel/setup.bash
    $ roslaunch my_robot world.launch

2- Use teleop_twist_keyboard for navigation (in a new terminal)

    $ cd ~/catkin_ws
    $ source devel/setup.bash
    $ rosrun teleop_twist_keyboard teleop_twist_keyboard.py

3- Launch amcl settings (in a new terminal)

    $ cd ~/catkin_ws
    $ source devel/setup.bash
    $ roslaunch my_robot amcl.launch 

4- Add the following settings to the Rviz Integration 

- Select odom for fixed frame
- Click the Add button and add RobotModel and your robot model should load up in RViz.
- add Map and select topic/map 
- add PoseArray and select topic/particlecloud

5- Control the robot with your keyboard

Sources:

- Udacity Robotics Software Engineer Nanodegree Project 3
- http://wiki.ros.org/amcl#Parameters
