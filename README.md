# Mini MobileArmBot with ROS2
![Overview of the project](https://github.com/LateefAkinola/Mini-MobileArmBot_with_ROS2/assets/105966848/1976c9bc-154f-488a-87d3-69c505874900)

## Description
In this project, we simply modeled a mobile base robot with a camera sensor to provide vision for navigation. A simple robot arm was then added on top of the mobile base for manipulation. 
Gazebo plugins were used:
- to configure the sensor
- the differential drive control for the rear wheels
- the joint state publisher and pose trajectory updates for the robot arm joints

## Installation
```bash
# Create your workspace directory
mkdir mobilearmbot_ws/
cd mobilearmbot_ws/

# Create your workspace directory
mkdir src/
cd src/
```
```bash
# Clone the repo
git clone https://github.com/LateefAkinola/Mini-MobileArmBot_with_ROS2.git
```
```bash
# Navigate back to the mobilearmbot_ws/ directory
cd ../..
```
```bash
# Build
colcon build

# Source the WS
source install/setup.bash
```

## Testing
```bash
# Execute the Launch File
ros2 launch mobilearmbot_bringup mobilearmbot_gazebo.launch.xml
```

## Future Work
This project can be further enhanced by adding grippers in the arm of the robot to help with diverse manipulation activities such as:
* Pick and Place;
* Material Handling;
* Assembly;
* Welding;
* Harvesting and Agricultural Tasks, etc.
