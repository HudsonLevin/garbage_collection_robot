# ROS & Gazebo Garbage Collection Robot Simulation 🗑️

A virtual robotics simulation framework developed within ROS (Robot Operating System) and Gazebo for automated trash retrieval and real-time kinematic validation.

## 💻 Tech Stack & Tools
- **Robotics Framework:** ROS 2
- **Simulation Environment:** Gazebo (Physics-based simulation)
- **Visualization:** RViz
- **Languages:** Python, CMake
- **3D Modeling:** SOLIDWORKS, Blender

## ⚙️ Core Modules
- **Kinematic Testing & 3D Assets:** Prepared and calibrated 3D robot links using SOLIDWORKS and Blender, ensuring precise joint origin points, coordinate frames, and rigid-body interactions.
- **Spatial Navigation & TF Tracking:** Integrated RViz to monitor robot states, sensor data streams, and TF (Transform) trees for real-time obstacle detection.
- **Teleoperation Interface:** Mapped and deployed a custom keyboard teleoperation node for responsive multi-axis navigation through virtual terrains.
- **Actuation & Manipulation:** Programmed Python scripts to translate software control inputs into physical simulation commands for precise robotic gripper manipulation.

## 🎥 Simulation Demos (Proof of Work)
Watch the system in action during our laboratory testing:
- [▶️ Main Garbage Collection Framework Demo](https://www.youtube.com/watch?v=pmQyw5dNUn0)
- [▶️ TF Tree & Spatial Tracking Visualization](https://youtu.be/YbC4uWs8SPo)
- [▶️ Laser/LIDAR Obstacle Scanning Mode](https://youtu.be/NGLglyEqCwk)
- [▶️ Responsive Multi-Axis Teleoperation](https://youtu.be/1A8YOOVMGqo)

## 📂 Repository Structure
- `articubot_one/` : Contains the core ROS 2 packages, URDF/XACRO models, and launch files for the simulation environment.

---

## 🚀 How to Run (Simulation Environment)

## 1. Prerequisites
Ensure you have **ROS 2 (Foxy or Humble)** and **Gazebo** installed on your Ubuntu system.

## 2. Setup and Build the Workspace
Clone this repository into the `src` folder of your ROS 2 workspace and build the package:
```bash
cd ~/ros2_ws/src
git clone [https://github.com/HudsonLevin/garbage_collection_robot.git](https://github.com/HudsonLevin/garbage_collection_robot.git)
cd ~/ros2_ws
colcon build --packages-select articubot_one
```

3. Source the Environment
After a successful build, source the ROS 2 environment and your local setup:
```bash
# Replace 'humble' with 'foxy' depending on your installed version
source /opt/ros/humble/setup.bash
source install/setup.bash
```

5. Launch the Simulation
Launch the Gazebo world and spawn the robot (replace [launch_file_name] with your specific launch file):
```bash
ros2 launch articubot_one [launch_file_name].launch.py
```
