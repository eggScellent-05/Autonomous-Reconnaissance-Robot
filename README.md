# Autonomous Reconnaissance Robot

A six-wheeled autonomous rover combining rocker-bogie suspension, onboard AI-based threat detection, and wireless mission communication, built as a 3-member team project in the Department of Mechanical Engineering, Amrita School of Engineering, Amritapuri.


📄 [Read the full paper](https://drive.google.com/file/d/1R930AxTggPM72jemCDEiTyJwj6zV0CZ5/view?usp=sharing)

----

## Overview

The rover uses a rocker-bogie suspension mechanism (the same design NASA has used on its Mars rovers) for stable, all-terrain mobility, and runs a lightweight custom-trained YOLOv8 Nano object detection model, exported to ONNX format, for real-time object/threat detection on a Raspberry Pi.

---

## Key Results

* **97.2% model size reduction** (419MB PyTorch → 11.6MB ONNX), enabling real-time inference (3-4 FPS) within a 1GB RAM constraint
* **MQTT-based wireless communication** for bidirectional, low-latency data transmission between the rover and a base station, including image alerts
* **Two-stage navigation validation:** a ROS2 Gazebo simulation using SLAM Toolbox and Nav2 for autonomous mapping in a simulated 40×40m environment, followed by physical hardware testing combining IMU-based dead-reckoning with ultrasonic-sensor obstacle avoidance

---

## Tech Stack

Python · ROS2 · YOLOv8 · ONNX Runtime · MQTT · Raspberry Pi

---

## Images

<img width="952" height="1269" alt="image" src="https://github.com/user-attachments/assets/656bc309-edc0-47ba-9d01-8fed10c8b102" />
The physical prototype, tested outdoors at Amrita Vishwa Vidyapeetham, Amritapuri.

---

## Status

This project was developed and tested as part of an academic paper (not yet published). This repository currently hosts the paper and project overview; full source code will be added as it's organized for public release.



