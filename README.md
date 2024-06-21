# Water-Level-Control-System
Simulink model of valve and pump control using PID regulator 

![model](https://github.com/Meg4Byte/Water-Level-Control-System/assets/121357383/d70053a0-5158-4ed0-84c8-cd2abd6a257d)


## Table of Contents
- [Introduction](#introduction)
- [Project Description](#project-description)
  - [Key Components](#key-components)
  - [Control Theory and Kinematics](#control-theory-and-kinematics)
  - [Implementation Steps](#implementation-steps)
- [Aim of project](#why-bother-with_this-project?)
- [Applications](#applications)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Cloning the Repository](#cloning-the-repository)
  - [Running the Code](#running-the-code)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The Ball Balancing Seesaw project aims to balance a ball on a beam using a servo motor for control. This project leverages the principles of classical control theory and kinematics to maintain the ball's position at the desired setpoint. It is a fundamental problem in control systems and robotics, providing a hands-on application of Proportional-Integral-Derivative (PID) control and sensor feedback integration.

## Project Description

The system consists of a beam mounted on a pivot, with a ball placed on the beam. A servo motor is connected to the pivot to adjust the beam's angle, thereby controlling the ball's position. The goal is to keep the ball at a specific position on the beam despite disturbances.

### Key Components

1. **Sensors**: Time of fligh sensor (e.g., VL53L0X) measures the distance of the ball from the pivot , providing real-time position feedback.
2. **Actuators**: A servo motor adjusts the beam's angle based on the control signals.
3. **Control Algorithm**: A PID controller computes the necessary adjustments to the beam angle to minimize the error between the ball's current position and the target position.

### Control Theory and Kinematics

- **Degrees of Freedom (DOF)**: The system is a 1 DOF problem, as it involves controlling the ball's position along one axis.
- **PID Control**: The PID controller uses the proportional, integral, and derivative terms to compute the control signal.The project uses PID but any control algorithm would do , the PID was chosen for it's simplicity.
- **Implementation Steps**: Refer to the [Implementation Steps](#implementation-steps) section for detailed steps on setting up and running the project.

## Why bother with this project?

- Real-time ball position feedback using an time of flight sensor , fundamentals of optical sensors , how do we measure and sample data using lasers , challenges and solutions.
- Derive a mathematical model most suitable for this project using Newtonian or Lagranian mechanics.Test your model with real life model and see the differences , how would you model non-idealities? 
- Design a PID controller that works according to your system requirements , hands of experience with settling time , steady-state error , overshoot , stability.How would you design a system to handle multiple disturbances?
- Actuator control . how do we choose actuator that is "good enough" for this project?What are some pros and cons of using servos?How would you handle deadband and slow response to fast disturbances or steady-state jitter? 
- It's a good feeling to make something with your hands from time to time , even though you can make such system from nothing (see the image above) there are real benefits if you decide to implement this using 3D modeling.

## Applications

- Educational purposes for learning PID control and robotics.
- Demonstrating principles of feedback control systems.
- Prototyping and development of automated positioning systems.
- Drone or airplace balancing can be aproximated using this model.
- Focal point for expanding to multiple DOF systems. 

## Installation

### Prerequisites

- Python 3.x
- Raspberry Pi (with Raspbian or compatible OS)
- Required libraries (e.g., VL53L0X Python library, RPi.GPIO)
- Special thanks to Gadgetoid for writting python module for VL53L0X ,check out the repository for more info https://github.com/Gadgetoid/VL53L0X-python

### Cloning the Repository

1. Open your terminal or command prompt.

2. Navigate to the directory where you want to store the project files.

3. Run the following command to clone the repository:

  ```bash
  git clone https://github.com/Meg4Byte/Ball-Balancing-Seesaw.git
  ```
  ```bash
  cd /Ball-Balancing-Seesaw/main
  ```

### Running the Code

In order to run the project do the following :

   1. ```bash
      chmod +x main.py

   2. ```bash
      python3 main.py
  
## Contributing

 If you'd like to contribute to this project, please follow these guidelines:
 
 Fork the repository on GitHub.
 Clone your forked repository to your local machine.
 Create a new branch for your feature or bug fix.
 Make your changes and commit them.
 Push your changes to your fork on GitHub.
 Create a pull request to submit your contribution.
   
## License 

This project is licensed under the MIT License. You are free to use, modify, and distribute this code at your own discretion.

## Contact

For questions or feedback, feel free to reach out at petnenadd_d@uns.ac.rs .

