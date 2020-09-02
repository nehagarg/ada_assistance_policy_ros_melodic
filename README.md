# ada_assistance_policy_ros_melodic

This repo contains a script that clones various repos needed to run ada_assistance_policy on ubuntu 18 with ros melodic in the directory ../ada_assistance_policy_ros_melodic_catkin_ws.

To run ada_assistance_policy code:
1. Install openrave using scripts provided at : https://github.com/crigroup/openrave-installation
2. Run create_ada_assistance_policy_catkin_ws.sh script provided in this repo
3. Go to ../ada_assistance_policy_ros_melodic_catkin_ws. Run catkin_make. To compile the code, you might also need to install libnlopt-dev, libnewmat10-dev and swig using apt
4. Run ada_assistance policy using command "rosrun ada_assistance_policy AdaSharedAutonomyGraspObjects.py -s -input mouse". You would need to provide Joy.msg at topic /ada/joy to control the arm.
