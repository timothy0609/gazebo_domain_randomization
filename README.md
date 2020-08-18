# gazebo_turtlebot_randomizer

1. download gazebo fundamental models

$ cd ~/.gazebo
$ git clone https://github.com/osrf/gazebo_models.git
$ mv gazebo_models models

2. copy turtlebot3_burger model to gazebo models file

$ cd ~/catkin_ws/src/gazebo_turtlebot_randomizer/gazebo_domain_randomization/gazebo_domain_randomizer/models
$ cp -R turtlebot3_burger ~/.gazebo/models/

3. make save direction

$ cd ~/.ros
$ mkdir -p result/dope/single/

4. build and run

$ cd ~/catkin_ws && catkin_make
$ roslaunch gazebo_domain_randomizer test.launch

please download scipy version 1.2.0.
