# 3D-RobotDesign-v1 (CONCEPT PHASE)

# Project Overview
This repository contains the initial 3D mechanical concept for a simple 3D-RobotDesign-v1. Designed via Tinkercad as part of the Smart Methods Summer Internship. The primary objective is to understand the end-to-end mechanical basics, system integration, and resource allocation constraints rather than building a highly complex model.

# System Architecture & Mechanical Design

Body Shape & Structure: A simple, lightweight rectangular chassis. This design provides a flat, stable platform to securely mount the system's core components (microcontroller, sensors, and battery) while keeping the Center of Gravity predictable.

Legs Design: Four symmetrical legs using basic geometric (oval) linkages. This minimizes material weight and reduces unnecessary load on the motors.

Joints & Degrees of Freedom: The system utilizes 2 joints per leg (Shoulder/Hip and Knee), totaling 8 joints for the entire robot. Keeping the Degrees of Freedom relatively low acts as a system constraint to optimize battery consumption and simplify the programming logic.

Motors Selection: Servo Motors are the optimal choice for this architecture. They provide the precise angle control required for a walking gait, unlike standard DC motors which rotate continuously.

# Physics & Movement Logic

Initial Torque Calculation (Concept): The highest torque demand is at the "Shoulder" joints. Torque equals Force multiplied by Distance. To ensure the robot can lift its own weight, the shoulder servos must have a torque rating greater than the total weight of the robot multiplied by the length of the upper leg segment.

Stability & Center of Gravity (CoG): The CoG is strategically placed in the dead center of the rectangular chassis. To maintain stability, the battery (the heaviest component) will be mounted precisely in the middle.

Proposed Walking Gait: The system will use a "Creep Gait" (moving one leg at a time). This ensures that three legs are always on the ground, keeping the CoG within the support triangle and preventing the robot from tipping over.

# Expected Mechanical Problems

Problem 1 (Friction): High friction between the upper and lower leg segments at the knee joint.

Problem 2 (Weight Imbalance): The robot tipping backward when accelerating.

