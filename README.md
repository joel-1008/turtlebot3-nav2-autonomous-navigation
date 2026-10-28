# TurtleBot3 Autonomous Navigation using ROS 2 Nav2

## Overview
This project demonstrates autonomous navigation of a TurtleBot3 in a Gazebo simulation using ROS 2 Jazzy and Nav2.

The robot navigates toward user-defined goals while displaying its planned path in RViz and avoiding obstacles.

## Technologies Used
- Ubuntu 24.04
- ROS 2 Jazzy
- TurtleBot3
- Gazebo Sim
- RViz2
- Nav2 Navigation Stack

## Features
- TurtleBot3 simulation in Gazebo
- Autonomous goal-based navigation
- Path planning visualized in RViz
- Obstacle avoidance using Nav2

## Setup Requirements
Install ROS 2 Jazzy and the required navigation packages:

```bash
sudo apt update
sudo apt install ros-jazzy-navigation2 ros-jazzy-nav2-bringup ros-jazzy-nav2-minimal-tb3-sim

```

Source the ROS 2 environment:
```bash
source /opt/ros/jazzy/setup.bash
```

## Launch Simulation

Start the TurtleBot3 simulation with Gazebo and RViz:

```bash
ros2 launch nav2_bringup tb3_simulation_launch.py headless:=False
```

## How to Test it

1. Wait for Gazebo and RViz to start.
2. Set the robot's initial position in RViz using 2D Pose Estimate, if required.
3. Select Nav2 Goal and click a destination on the map.
4. Observe the planned path in RViz and the robot's movement in Gazebo.
5. Test different goals and verify obstacle avoidance.

## Challenges and Learnings

- Learned to launch and inspect a ROS 2 simulation.
- Used Nav2 lifecycle states to troubleshoot navigation startup.
- Practiced setting the robot's initial pose and navigation goals in RViz.
- Observed path planning and obstacle avoidance during autonomous navigation.

## Demonstration

A screen recording demonstrating autonomous navigation is included in this repository.

Demo video: [Demo-Turtlebot.mp4](Demo-Turtlebot.mp4)

The video shows the TurtleBot3 navigating toward a goal in Gazebo, with the planned path and navigation displayed in RViz.
