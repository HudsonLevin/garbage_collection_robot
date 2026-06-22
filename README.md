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
