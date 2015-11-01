TME Subsomption
===============

Source files and questions for a practical course on the subsumption architecture.

Content
=======

subsomption/ : directory containing the required ROS nodes. 

Usage & installation
====================

Create a link in your catkin dir and launch catkin_make (update with your dir):

    cd ~/catkin_ws/src
    ln -s ~/git/TME_subsomption/subsomption
    cd ~/catkin_ws
    catkin_make

To use it, launch:

   rosrun subsomption subsomption_architecture.py 10

The number tells how many levels you consider (here 10).

example.py contains an example of module to be used in this architecture.

The modules will be launched like that:

    rosrun subsomption example.py




