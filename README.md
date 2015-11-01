TME Subsomption
===============

Source files and questions for a practical course on the subsumption architecture.

Requires the fastsim simulation. You can use it to control a turtlebot with the fastsim_to_turtlebot ROS node available here: https://github.com/doncieux/ros_misc.git

Dependencies
============

* libfastsim (https://github.com/jbmouret/libfastsim)
* ros_fastsim (https://github.com/jbmouret/ros_fastsim)

Content
=======

subsomption/ : directory containing the required ROS nodes. 

Usage & installation
====================

lib fastsim and ros_fastsim need to be installed.

Create a link in your catkin dir and launch catkin_make (update with your dir):

    cd ~/catkin_ws/src
    ln -s ~/git/TME_subsomption/subsomption
    cd ~/catkin_ws
    catkin_make

Before using the subsumption architecture, you need to launch the ros_fastsim node:
    cd ~/catkin_ws/src/subsomption/envs
    roslaunch fastsim.launch

To use it, launch:

   rosrun subsomption subsomption_architecture.py 10

The number tells how many levels you consider (here 10).

example.py contains an example of module to be used in this architecture.

The modules will be launched like that:

    rosrun subsomption example.py




