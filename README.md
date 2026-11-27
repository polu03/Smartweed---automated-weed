# Smartweed---automated-weed detection 

Automated weed detection and removal system for agriculture, built with edge AI and robotics. The goal is chemical-free weed management for small and medium farms.

## Overview

Smartweed captures images of crop rows, detects weeds with a trained object-detection model running on an edge device, and sends the weed position to a mechanical actuator that removes it. All processing happens on the device, so no internet or cloud connection is needed in the field.

## How It Works (High Level)

1. Capture: A camera captures live images of the crop row.
2. Preprocess: Frames are resized and cleaned up for the model.
3. Detect: A YOLOv11 model detects and locates weeds.
4. Act: A microcontroller drives a linear actuator to remove the detected weed.

## Hardware

- NVIDIA Jetson Xavier NX (edge AI processing)
- Arducam IMX477 12MP camera (image capture)
- ESP32 microcontroller (actuator control)
- Linear actuator (weed removal)
- RPLiDAR A2M12 (obstacle detection and navigation)
- 24V battery with DC-DC converters (power)
- Cooling system and chassis

## Software

- Python, OpenCV
- YOLOv11 (trained on Google Colab)
- TensorRT (inference optimization)
- Arduino / ESP32 firmware

## Status

Work in progress. Code and documentation will be added to this repository.

## Author

Sarvada Shahapure