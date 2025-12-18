---
tags:
  - "#setup"
  - "#hardware"
  - "#computer"
---
## Ubuntu 24.04
---
> **TLDR:** Install ROS jazzy, Install required packages, clone
### ROS 2:  Jazzy Jalisco 
Install walk through link is [here](https://docs.ros.org/en/jazzy/Installation/Ubuntu-Install-Debs.html). Make sure it is the guide for Ubuntu (deb packages) and not the guide for installing by building from source or binaries. 

> I also recommend installing `ros-jazzy-desktop` when it is time to chose a version.
### Required Packages 
Some of the packages i have used so far can be simply installed by running `sudo apt install`, others have to be cloned from GitHub and built due to not being on the ROS Index.
#### Debian Packages (apt)
Here are some of the packages that are required to run the simulated robot + interact with the hardware. Install each one by running `sudo apt install <package_name>`.

Required Packages:
- `ros-jazzy-ros2-control`
- `ros-jazzy-ros2-controllers`
- `ros-jazzy-navigation2`
- `ros-jazzy-nav2-bringup`
- `ros-jazzy-nav2-minimal-tb`
- `ros-jazzy-ros-gz`

Useful Packages:
- `ros-jazzy-slam-toolbox`
- `ros-jazzy-turtlebot3
#### Built Packages
All you have to do to build these package is clone them to the directory `~/ros2_ws/src`,  move back into the root of your ROS workspace and run `colcon build --symlink-install`. Some of these packages might throw a warning or two, but it is fine and does not effect anything.
## Windows / MacOS 
---
