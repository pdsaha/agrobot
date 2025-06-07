# AgroBot - Affordable Weed Detection and Elimination

**AgroBot** is an affordable, AI-powered robotic system designed to autonomously detect and eliminate weeds in agricultural fields. It integrates **computer vision**, **machine learning (YOLOv5)**, and **ROS-based navigation** to provide a sustainable, low-cost alternative to manual weeding and chemical herbicide overuse.

## Features

* 🚜 Autonomous navigation using IMU-based odometry and EKF sensor fusion
* 🎯 Real-time weed detection with YOLOv5 object detection
* 💧 Targeted spraying system to minimize chemical usage
* 🧠 ROS Noetic architecture with Docker-based deployment
* 💻 CAD-designed chassis and URDF for robot simulation and visualization

## Components

* Raspberry Pi 5 (8GB) running ROS Noetic
* ESP32 microcontroller for motor and sensor control
* MPU6050 IMU for localization
* Diaphragm pump and servo-controlled nozzle
* YOLOv5 trained on a weed detection dataset (Kaggle)

## Getting Started

1. **Hardware Setup**: Assemble the bot as per CAD design, connect sensors, camera, and motors.
2. **Software Deployment**:

   * Flash firmware on ESP32
   * Run ROS nodes in Docker container on Raspberry Pi
3. **Operation**:

   * Fill pesticide container
   * Power on and place on level surface
   * Bot starts autonomous detection and spraying

## Performance

* **mAP50**: 0.763 (YOLOv5 on test set)
* **Inference Time**: 0.18–0.20 ms (256x256 images)
* Effective in reducing manual labor and chemical input costs
