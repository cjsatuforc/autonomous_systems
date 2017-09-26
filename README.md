Autonomous Systems
===

This repository holds code and resources for the Autonomous Systems course by Prof. Pedro Lima, Prof. Rodrigo Ventura and M.Sc. Oscar Lima Carrion
which takes place at Instituto Superior Tecnico, Lisboa.

NOTE: The course expects you to have installed Ubuntu 16.04 and ROS Kinetic.

Please follow these instructions:

Installation instructions
===

Install git on your system:

        sudo apt-get install git

Navigate to your home folder:

        cd $HOME

Clone the repository:

        git clone https://github.com/socrob/autonomous_systems.git

Setup catkin workspace and scripts structure (one time only)
===

A partial documentation of this can be found [here](http://wiki.ros.org/catkin/Tutorials/create_a_workspace) and [here](http://catkin-tools.readthedocs.io/en/latest/index.html)

For convenience and to save you time you can run a script to perform the instructions on this block by doing:

        bash ~/autonomous_systems/resources/auton_sys_setup.sh

If you have used the automated script you can skip to section Lab1 below.

If you decide to do it manually (for didactic purposes) then please continue:

1. Create a folder for your ros workspace in your system:

        mkdir -p ~/ros_ws/src

2. Install python catkin tools (to be able to compile with the new catkin build system, instead of catkin_make which is the old one)

        sudo apt-get install python-catkin-tools

3. Source (enable) ROS on your system (only one time, this line should not be there on your .bashrc as it will be bashed by the scripts structure)

        source /opt/ros/kinetic/setup.bash

4. Compile your workspace:

        cd ~/ros_ws && catkin build

5. Add lines of code to your .bashrc to source the scripts configuration files

        echo "# personal config starts here" >> ~/.bashrc && echo "source ~/scripts/permanent.sh" >> ~/.bashrc

6. Copy scripts folder to your home directory:

        cp -r ~/autonomous_systems/resources/scripts $HOME

7. Source your new scripts structure:

        source ~/.bashrc

Lab1
===

Please open lab1 folder to access the lab slides and follow the instructions for the practical exercise. There is README.md file inside.

lab2
===

Lab 2 material will be published in this repository soon.

To get updates you can do:

        git pull origin master

Questions
===

Please post your questions under:

        https://github.com/socrob/autonomous_systems/issues

By creating an issue, so that we can all benefit from the answers.

Thanks!

Resources
===

Inside resources folder there is script folder that you can copy on your system home folder to facilitate
your work with some nice features such as: color syntax highlight scripts and alias, suggested programs to install,
loading relevant ROS ennvironment variables, etc.
