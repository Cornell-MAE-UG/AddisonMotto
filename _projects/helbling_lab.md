---
layout: project
title: Helbling Robotics Research Lab
description: Graduate researcher in a Cornell laboratory
summary: Contributing a dynamic braking mechanism to Gammabot, a flapping-wing robot designed for controlled locomotion along the air-water interface.
order: 2
technologies: [Onshape, Research & Literature Review, Experimental Design & Testing, Carbon Fiber Manufacturing, Data Post-Processing]
image: /assets/images/gammabot1.png
---


## Overview

I joined the Helbling Robotics Research Lab as part of my **Systems Engineering M.Eng. project**, working on **Gammabot**, a small (<1 gram) flapping-wing robot designed to move along the air-water interface.

A major challenge with the current robot is that its wing-based locomotion can only drive it forward. It cannot actively reverse direction, which makes stopping and position control difficult. My project focuses on developing and testing a braking mechanism that can slow the robot down and, eventually, help it remain relatively still while the wings continue flapping.

The long-term goal is for this braking mechanism to be actuated so that multiple robots can pause and communicate with each other by sending and reading vibration frequencies across the water surface caused by their flapping wings.

---

## Project Goal

The goal of my work is to design, prototype, and experimentally evaluate a lightweight braking mechanism for Gammabot.

The brake needs to:

* Increase drag enough to reduce stopping distance.
* Stay lightweight and compact enough for the robot.
* Work at the air-water interface without disrupting locomotion.
* Eventually be actuatable so the robot can slow down or hold position.
* Support future communication between robots through water-surface vibrations.

---

## Experimental Setup

To test braking performance, we used a controlled experimental setup with:

* A **low-drag magnetic rail** to guide the robot's motion.
* A **pulley system** to accelerate the robot before testing.
* A **high-speed camera** to record the robot's motion.
* Motion-tracking software to extract position, velocity, and speed decay over time.

This setup allowed us to compare braking behavior at different brake depths and estimate how much each configuration reduced the robot's stopping distance.

**[Insert image of experimental setup here]**

---

## Testing Approach

Our original plan was to accelerate the robot with the brake raised, then pull a pin after acceleration so the brake would drop into the water. This would have better represented how an actuated brake might work in the future.

However, we ran into two major issues. First, the pin-pull mechanism reduced the robot's speed during release, making the data less reliable. Second, after the pin was pulled, the brake sometimes did not have enough weight to break the water's surface tension and fully deploy.

Because of this, we changed the test approach. Instead of deploying the brake after acceleration, we accelerated Gammabot with the brake already down and measured its velocity decay. We then compared the braking distance across different brake depths.

This method still gave us useful data, but it likely gives a conservative estimate of braking performance. Since the brake was down during acceleration, the added drag and added mass probably made the robot slower before the actual decay measurement began. A deployed-after-acceleration brake would likely perform better than what we measured.

**[Insert brake depth comparison graph here]**

---

## Deliverables

For this project, my main deliverables were:

* A lightweight brake prototype for Gammabot.
* An adjustable test setup for evaluating brake depth.
* Experimental trials comparing multiple brake configurations.
* Motion-tracking data showing position, velocity, and speed decay.
* Braking-distance comparisons across brake depths.
* Recommendations for future brake geometry and actuation improvements.

---

## Results

The brake produced a clear change in Gammabot's motion and increased the rate at which the robot slowed down. By testing different brake depths, we were able to compare how strongly each configuration affected stopping distance.

The results showed that even a small passive brake can meaningfully affect the robot's motion at the air-water interface. This supports the broader idea that a future actuated brake could help the robot slow down, hold position, and communicate with other robots while the wings are still flapping.

**[Insert velocity decay plot here]**

**[Insert stopping distance comparison here]**

---

## Next Steps

The next step is to improve the brake geometry so it deploys more reliably and breaks through the water surface more easily. Future designs could explore different brake shapes, sharper leading edges, or small added features that help overcome surface tension.

Another important next step is adding fins or stabilizing features to reduce yaw during braking. If the brake introduces too much rotation, it becomes harder to control the robot's final position and orientation.

Longer term, the goal is to develop an actuated version of the brake that can be triggered on command. This would allow Gammabot to actively slow down or remain relatively still while flapping, which is important for future robot-to-robot communication through vibration frequencies on the water surface.

---

## What I Learned

This project brought together a lot of the engineering work I enjoy: mechanical design, testing, modeling, and system-level problem solving. The brake itself is small, but the full system is complicated because the robot, water surface, flapping wings, rail setup, and measurement system all affect the final results.

It was also a good reminder that a design does not just need to work in CAD. It needs to deploy reliably, survive testing, produce measurable data, and fit into the larger goal of the robot.
