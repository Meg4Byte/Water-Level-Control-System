# Water-Level-Control-System

Simulink model of valve and pump control using PID regulator 

![model](https://github.com/Meg4Byte/Water-Level-Control-System/assets/121357383/d70053a0-5158-4ed0-84c8-cd2abd6a257d)

![output](https://github.com/Meg4Byte/Water-Level-Control-System/assets/121357383/af8c1d79-f7f4-4e35-af71-204b1473d1b1)

## Table of Contents
- [Introduction](#introduction)
- [Project Description](#project-description)
  - [Parts of the System](#parts-of-the-system)
  - [Control Theory Overview](#control-theory-overview)
  - [Implementation Steps](#implementation-steps)
- [Project Objectives](#project-objectives)
- [Applications](#applications)
- [Installation](#installation)
  - [Prerequisites](#prerequisites)
  - [Cloning the Repository](#cloning-the-repository)
  - [Running the Model](#running-the-model)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The Water-Level-Control-System project focuses on maintaining a desired water level in a tank by controlling a pump using a PID regulator. This project demonstrates the use of Simulink for modeling and simulating control systems, providing insights into the practical application of PID control in a non-linear system.

## Project Description

The system models a water tank where the water level is controlled by adjusting the voltage to a pump. The relationship between the input voltage and the water level is governed by the non-linear differential equation:

\[ A \frac{dh}{dt} = bV - a\sqrt{h} \]

where:
- \( V \) is the input voltage controlling the pump,
- \( h \) is the height of the water (water level in the tank),
- \( A \) is the surface area of the tank,
- \( b \) and \( a \) are constants.

This non-linear system cannot be solved using linear system methods like Laplace transforms. The PID controller is used to regulate the water level despite the system's non-linearities and external disturbances.

### Key Components

1. **Pump**: Adjusts the water level in the tank based on the input voltage.
2. **Tank**: The container where the water level is controlled.
3. **PID Controller**: Regulates the voltage to the pump to maintain the desired water level.
4. **Sensors**: Measure the current water level and provide feedback to the controller.

### Control Theory

- **PID Control**: The PID controller uses proportional, integral, and derivative terms to compute the control signal. The controller parameters are tuned to achieve the desired performance in terms of settling time, steady-state error, and stability.
- **Non-linear Modeling**: The system's non-linear behavior is modeled using the given differential equation. Band-limited white noise is added in the feedback path to simulate sensor noise, and a step input signal is used to represent disturbances in the water flow.

### Implementation Steps

1. Model the system using Simulink, incorporating the differential equation for water level dynamics.
2. Design and tune the PID controller to achieve desired control performance.
3. Simulate the system and analyze the response to various disturbances and noise.

## Project Objectives

- Understand and implement real-time water level control using a PID regulator.
- Learn about non-linear system modeling and control.
- Explore the effects of sensor noise and disturbances on system performance.
- Gain practical experience with Simulink for control system design and simulation.

## Applications

- Educational tool for learning about PID control and non-linear systems.
- Demonstration of control theory principles in practical applications.
- Basis for developing more complex automated water management systems.
- Model for understanding and designing similar control systems in different domains.

## Installation

### Prerequisites

- MATLAB with Simulink
- Basic understanding of control systems and differential equations

### Cloning the Repository

1. Open your terminal or command prompt.
2. Navigate to the directory where you want to store the project files.
3. Run the following command to clone the repository:

  ```bash
  git clone https://github.com/Meg4Byte/Water-Level-Control-System.git
