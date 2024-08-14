# Vision-Based-Pick-and-place


## Project Overview

This project is focused on developing a vision-based pick-and-place application using a 2D color camera and a cobot UR5e from Universal Robots. The project introduces the integration of vision systems into robotic operations, particularly for tasks where the positions and orientations of objects are not pre-determined, such as bin picking. The application simulates the process in a virtual environment before transitioning to real-world hardware, highlighting the challenges and intricacies of vision-based robotic manipulation.

## Aim of the Project

The primary aim of this project is to:

1. **Learn Vision-Based Object Recognition**: Utilize a 2D color camera (Azure Kinect DK) to recognize and differentiate objects based on color.
2. **Compute Gripping Poses**: Determine the appropriate gripping pose (position and orientation) for objects located on a flat surface.
3. **Simulate Pick-and-Place Operations**: Implement and simulate the pick-and-place task in RoboDK to validate the process before deployment.
4. **Transfer to Real Hardware**: Apply the developed simulation to a real UR5e cobot, transferring the pick-and-place operation from a virtual environment to a physical setup.
5. **Understand Real-World Challenges**: Gain insight into the challenges associated with vision-based robotic applications in real-world scenarios, such as lighting variations, object occlusion, and camera calibration.

## Key Points of the Project

### 1. Introduction to Vision-Based Robotic Applications

- **Industrial Applications**: Vision-based pick-and-place operations are common in automated assembly lines where objects are randomly oriented, requiring vision sensors to identify and localize them.
- **Learning Objectives**:
  - Understand the role of vision systems in robotic automation.
  - Learn to integrate vision data with robotic control systems for dynamic object manipulation.

### 2. Installation and Setup

- **Required Software**:
  - **Matlab**: Primary tool for processing vision data and calculating gripping poses.
    - Tested with Matlab v2021a (v2022a also works with minor issues).
    - Requires the Image Processing Toolbox.
  - **Machine Vision Toolbox**:
    - Essential for vision-based operations in Matlab.
    - Download from [Peter Corke's Toolbox](https://petercorke.com/toolboxes/machine-vision-toolbox/).
  - **RoboDK Simulation Environment**:
    - Used for simulating the pick-and-place operation.
    - Tested with version 5.5.2 (64bit).
  - **Files**:
    - Download the necessary Matlab and RoboDK simulation files from the provided e-learning platform.
  
### 3. High-Level Task Description

- **Vision-Based Object Recognition**:
  1. The robot captures an image of its workspace using a camera mounted on its flange.
  2. The system processes the image to identify colored blocks (red, green, blue) and computes their positions and orientations within the workspace’s coordinate system.
  
- **Pick-and-Place Sequence**:
  1. The robot picks up the colored blocks in the following sequence: red, green, blue.
  2. The blocks are stacked in the correct order at a predefined position on the table.
  
### 4. Simulation and Real-World Implementation

- **Simulation Phase**:
  - **Objective**: Simulate the pick-and-place operation using RoboDK to ensure the system performs the task accurately in a virtual environment.
  - **Outcome**: Validate the robot’s ability to recognize, pick, and place the objects in the correct order.
  
- **Real-World Phase**:
  - **Objective**: Transfer the simulation results to a real UR5e cobot equipped with the Azure Kinect DK camera.
  - **Challenges**: Address real-world issues such as camera calibration, lighting conditions, and physical object handling.

### 5. Challenges in Vision-Based Applications

- **Real-World Complexities**: Unlike simulations, real-world environments present unpredictable variables like lighting changes, object occlusions, and inaccuracies in object detection.
- **Camera Calibration**: Ensuring that the camera’s coordinate system aligns perfectly with the robot’s workspace is crucial for accurate object localization.
- **Gripping Precision**: The computed gripping pose must be accurate to prevent the robot from missing or misaligning objects during the pick-and-place task.

## Getting Started

### Prerequisites

- Basic understanding of robotics and Matlab.
- Familiarity with image processing concepts is helpful but not required.

### Installation

1. Install Matlab and the Image Processing Toolbox.
2. Download and install the Machine Vision Toolbox from [Peter Corke's website](https://petercorke.com/toolboxes/machine-vision-toolbox/).
3. Download and install RoboDK, and obtain a license if required.
4. Download the necessary Matlab and simulation files from your e-learning platform.

### Running the Simulation

1. Load the simulation files in RoboDK.
2. Run the Matlab script to process the vision data and compute the gripping poses.
3. Simulate the pick-and-place operation in RoboDK to verify the system’s functionality.
4. Transfer the simulation to the UR5e cobot for real-world testing.

## Conclusion

This project provides a comprehensive introduction to vision-based robotic operations, from initial simulation to real-world implementation. By completing this project, participants will gain valuable skills in integrating vision systems with robotic manipulators, a critical competency in modern automation. The project also highlights the importance of simulation in validating robotic tasks before physical deployment, thereby reducing the risk of errors and improving overall system efficiency.

