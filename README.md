# Configure-Python-3-in-ROS-Melodic-and-early-version

Python 3 users in ROS Melodic and earlier: note, if you are building ROS from source to achieve Python 3 compatibility, and have setup your system appropriately (ie: have the Python 3 versions of all the required ROS Python packages installed, such as catkin) the first catkin_make command in a clean catkin workspace must be:

## Ensure that catkin_pkg is installed and up to date. You can install it using pip:
 pip install -U catkin_pkg
## Ensure that pip is installed:
 sudo apt-get install python3-pip
## Then, install the catkin_pkg package using pip3:
  pip3 install -U catkin_pkg
## This will configure catkin_make with Python 3:
 catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3
## You may then proceed to use just catkin_make for subsequent builds.


# Reference 
https://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment
