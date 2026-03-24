# Kinova Unseen Object Grasping Demo

A ROS-based demo for grasping previously unseen objects with a Kinova robotic arm using single-camera perception, manual calibration, and motion execution.

This project was built as a practical robotics demo to integrate perception, camera-to-robot calibration, and robot motion into an end-to-end grasping workflow.

## Overview

The goal of this project is to demonstrate a simple unseen-object grasping pipeline on a real robot system.

The demo combines:
- a Kinova robotic arm
- ROS-based system integration
- single-camera perception
- ArUco-assisted transform calibration
- motion execution for top-down grasping

The system is designed as a practical demo rather than a fully general grasping framework. It focuses on getting a complete perception-to-action pipeline running on real hardware.

## What this project demonstrates

- End-to-end integration of robot control and perception in ROS
- Camera-to-robot transform setup for real-world deployment
- Object approach and grasp execution on a Kinova platform
- Practical handling of deployment issues such as system faults and reinitialization

## System workflow

The demo follows this high-level process:

1. Launch the robot and perception system
2. Set up or verify camera-to-robot transforms
3. Detect the target object / target frame
4. Move the robot above the object
5. Move down for grasp execution
6. Restart or reselect targets when needed

## Repository structure

```text
.
├── config/          # Configuration files
├── launch/          # ROS launch files
├── pic/             # Demo images / setup reference images
├── src/             # Python source code
├── CMakeLists.txt
├── package.xml
└── README.md