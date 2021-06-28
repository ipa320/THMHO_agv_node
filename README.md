# betterfactory_agv_firos

## Installation
```
# Create a new ROS workspace
mkdir -p catkin_ws/src && cd catkin_ws/src

# Download the repository
git clone https://github.com/ipa-rar/betterfactory_agv_firos.git

# Download dependencies
cd betterfactory_lidar_firos
wstool init ~/catkin_ws/src/betterfactory_agv_firos
wstool merge ~/catkin_ws/src/betterfactory_agv_firos/betterfactory_lidar_firos.rosinstall 
wstool up
cd ..

# Install dependencies 
rosdep update && rosdep install --from-paths ~/snp_demo_ws/src --ignore-src


cd ~/catkin_ws && catkin_make
source ~/catkin_ws/devel/setup.bash

```
