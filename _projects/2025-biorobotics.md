---
layout: project
title: Biorobotics
description: Autonomous agricultural robot with vision-based sorting, custom manipulators, and grid navigation
technologies: Arduino, Raspberry Pi, TFLite, CAD, 3D Printing, Python
image: assets/images/biorobotics-robot.png
---

## Biorobotics Project Overview

For BEE 5900, my team designed an autonomous robotic system for agricultural environments that could navigate a grid, identify plant conditions, and perform selective handling and sorting tasks. The robot combined mobility, perception, manipulation, and storage into a modular platform built under strict physical, time, and budget constraints.

## System Approach

The robot architecture divided responsibilities between an Arduino and a Raspberry Pi. The Arduino handled real-time drivetrain and arm control, while the Raspberry Pi managed camera input, image processing, and machine-learning-based classification of plant characteristics such as size and condition. This separation allowed the robot to move through the arena, detect targets, and execute the appropriate pick, deposit, or sort action in a structured workflow.

## Hardware Design

The mechanical system included a rigid chassis, an articulated robotic arm with a claw, and custom 3D-printed storage boxes. The chassis used omni-directional wheels for precise movement in a confined environment, while the claw incorporated foam and rubber on the gripping surfaces to improve traction and reduce slippage. The herb and seed boxes were designed with ramps, chamfers, and lightweight cutouts to improve deposition reliability and reduce material use.

## Software and Logic

The navigation software was built to traverse a 4x4 grid of 16 bases within the competition time limit while maintaining accurate positioning for arm operations. The object-detection system classified target states in real time and mapped them to treatment actions through a serial interface, supporting decisions such as removing bad plants, extracting plants from doubles, or replanting seeds. The final competition logic relied on a state machine to coordinate navigation, vision, and arm movement while preserving collision safety and timing constraints.

## Performance and Results

Pre-competition testing validated the core subsystems, including turn accuracy, stepper precision, PWM positioning, and the vision-to-serial-to-action pipeline. In competition, the system successfully completed the right-side plant pickup and deposit cycle, but the left-side traversal was not implemented, which limited full dual-target completion. The report identifies the main limitation as unidirectional path planning rather than individual subsystem failure.

## Personal Contributions

My contributions focused on the integration of mechanical design, control logic, and report development. I worked on the robot’s modular design approach, helped support the division between Arduino and Raspberry Pi tasks, and contributed to the documentation of the hardware and software workflow. I also helped explain the testing limitations and the remaining path-planning improvements needed for full autonomous operation.

## Selected Figures

- Front view of the fully assembled arm and claw CAD model.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-arm-front.png"
       alt="Biorobotics arm front CAD"
       style="max-width: 350px; height: auto;">

- Top view of the fully assembled arm and claw CAD model.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-arm-top.png"
       alt="Biorobotics arm top CAD"
       style="max-width: 350px; height: auto;">

- Back view of the fully assembled arm and claw CAD model.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-arm-back.png"
       alt="Biorobotics arm back CAD"
       style="max-width: 350px; height: auto;">

- Front view of the CAD model for the herb storage box.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-herb-box-front.png"
       alt="Biorobotics herb box front CAD"
       style="max-width: 350px; height: auto;">

- Top view of the CAD model for the herb storage box.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-herb-box-top.png"
       alt="Biorobotics herb box top CAD"
       style="max-width: 350px; height: auto;">

- Front view of the CAD model for the seed storage box.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-seed-box-front.png"
       alt="Biorobotics seed box front CAD"
       style="max-width: 350px; height: auto;">

- Side view of the CAD model for the seed storage box.

  <img src="/fa25-portfolio-yc852/fa25-portfolio-yc852/assets/images/biorobotics-seed-box-side.png"
       alt="Biorobotics seed box side CAD"
       style="max-width: 350px; height: auto;">