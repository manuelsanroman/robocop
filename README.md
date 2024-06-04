# ROBOCOP Project

This repository contains the code for the ROBOCOP project developed by Manuel, Vera, Zane, and Tse Wei Yu. The project involves a robot named MCLANE designed to navigate an environment by following lines and avoiding obstacles.

## Table of Contents
- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Main Logic](#main-logic)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The ROBOCOP project aims to create an autonomous robot capable of navigating an environment using a combination of line-following and object detection. The main features include:
- Following a line when no object is detected.
- Performing a 180º turn when an object is detected.

## Getting Started

To get started with the ROBOCOP project, clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/robocop.git
```

Navigate to the project directory:
```bash
cd robocop
```

## Dependencies

The project relies on the following dependencies:

ROS (Robot Operating System)
OpenCV
Other dependencies as specified in requirements.txt
To install the necessary dependencies, run:

```bash
pip install -r requirements.txt
```

## Usage
To run the project, use the following command within your ROS environment:

```bash
rosrun robocop main.py
```

This will start the robot's main logic and enable the line-following and object detection features.

## Main Logic
The main logic of the robot is described as follows:

1. Line Following: If no object is detected, the robot follows a line.
Topic: /camera/color/image_raw

2. Object Detection: If an object is detected, the robot performs a 180º turn.
Topic: /scan

The robot continuously checks for objects and switches between the two modes based on the presence of obstacles.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.
