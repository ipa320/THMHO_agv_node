# betterfactory_agv_firos

## Installation
```
# Create a new ROS workspace
mkdir -p catkin_ws/src && cd catkin_ws/src

# Download the repository
git clone https://github.com/ipa320/THMHO_agv_node.git

# Download dependencies
cd THMHO_agv_node
wstool init ~/catkin_ws/src/THMHO_agv_node
wstool merge ~/catkin_ws/src/THMHO_agv_node/THMHO_agv_node.rosinstall 
wstool up
cd ..

# Install dependencies 
rosdep update && rosdep install --from-paths ~/catkin_ws/src --ignore-src


cd ~/catkin_ws && catkin_make
source ~/catkin_ws/devel/setup.bash

```
