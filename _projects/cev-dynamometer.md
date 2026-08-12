---
layout: project
title: Electric Vehicle Dynamometer
description: Cornell Electric Vehicles test hardware
summary: Built a low-cost dynamometer from available team hardware to measure motor output power and support motor-controller validation.
order: 3
technologies: [Mechanical Design, Test Fixtures, Load Cell Measurement, Tachometer Instrumentation, Braking Systems, Data Reduction]
image: /assets/images/cev-dynamometer-test-stand.png
---

## Low-Cost Motor Power Test Stand

For Cornell Electric Vehicles, I designed and built a small dynamometer to help the motor controller team verify motor output power during bench testing. The goal was to create a practical test fixture using parts already available in the shop, rather than relying on a commercial dynamometer or waiting for a purpose-built system.

The final setup used a structural aluminum frame, a motor mount, shaft supports, recycled brake hardware from one of the team's older vehicles, a tachometer for rotational speed, and a load cell to measure braking force. A small hand wheel adjusted hydraulic brake pressure so the motor could be loaded in a controlled and repeatable way during testing.

<div style="display: flex; flex-direction: column; align-items: center; gap: 42px; margin: 35px 0 15px 0;">

  <div style="text-align: center; width: 100%;">
    <img src="{{ "/assets/images/cev-dynamometer-test-stand.png" | relative_url }}"
         alt="Cornell Electric Vehicles dynamometer test stand with motor, brake rotor, tachometer, and load cell"
         style="width: 100%; max-width: 900px;">
    <p style="font-size: 13px; margin-top: 8px; color: #666;">Full test stand with motor, shaft supports, brake rotor, tachometer, and load cell fixture.</p>
  </div>

  <div style="text-align: center; width: 100%;">
    <img src="{{ "/assets/images/cev-dynamometer-brake-assembly.png" | relative_url }}"
         alt="Close view of bicycle brake caliper, rotor, hydraulic line, and hand wheel adjustment on the dynamometer"
         style="width: 100%; max-width: 900px;">
    <p style="font-size: 13px; margin-top: 8px; color: #666;">Brake assembly and hand-wheel adjustment mechanism used to vary load on the motor.</p>
  </div>

</div>

## Measurement Approach

The dynamometer measured power by combining rotational speed with brake reaction force. A tachometer recorded motor speed while the brake assembly applied load to the rotating shaft. The braking torque was calculated from the known lever arm length and the force measured by the load cell:

<p style="text-align: center; font-size: 1.15rem; margin: 30px 0;">
  torque = load cell force &times; lever arm length
</p>

Once torque and rotational speed were known, motor output power could be calculated and compared against expected motor-controller behavior. This gave the electrical team a simple way to validate commanded output, observe performance under load, and identify whether the motor-controller system was producing the expected mechanical power.

## Design Constraints

A major part of the project was making the system work with available components. The brake hardware came from an older team vehicle and was originally intended for bicycle-style braking, so the fixture had to adapt those parts into a stable bench-test configuration. I designed the frame and mounting layout around the hardware on hand, focusing on stiffness, alignment, adjustability, and ease of assembly.

The hand-wheel adjustment was added to make loading easier during testing. Instead of making small changes directly at the brake assembly, the operator could gradually increase braking force and watch the speed and load-cell response in real time.

<div style="text-align: center; width: 100%; margin: 38px 0 12px 0;">
  <img src="{{ "/assets/images/cev-dynamometer-cad.png" | relative_url }}"
       alt="CAD model of the Cornell Electric Vehicles dynamometer fixture"
       style="width: 100%; max-width: 900px;">
  <p style="font-size: 13px; margin-top: 8px; color: #666;">CAD model showing the fixture layout, shaft supports, brake rotor, lever arm, and load-cell mounting location.</p>
</div>

## Engineering Challenges

### Brake Pad Overheating

One of the main issues going forward is heat buildup in the brake pads. Because the brake dissipates the motor's mechanical output as frictional heat, sustained testing can quickly push the pads and rotor beyond the conditions they were designed for. As the pads heat up, their coefficient of friction can change, which makes the applied load less consistent and reduces measurement repeatability. Excessive heat can also accelerate pad wear, cause brake fade, and potentially damage nearby components or create an unsafe test condition.

A future version would benefit from better thermal management, such as a larger rotor, a more robust brake system, cooling airflow, shorter test intervals, or temperature monitoring so data can be filtered or paused when the brake system approaches its thermal limits.

### Hydraulic Pressure Loss

Another limitation was the hydraulic brake system. The brake fluid leaked and the system lost pressure over time, which meant the brakes had to be re-bled frequently. This made the setup harder to use and reduced confidence in repeatability between tests because the same hand-wheel position could produce a different clamping force after pressure loss.

Future improvements would include replacing worn fittings or seals, improving line routing, using a more reliable master cylinder or caliper, and adding a more direct pressure measurement so the brake state could be monitored during a test.

## Outcome

The dynamometer provided a useful low-cost test platform for the Cornell Electric Vehicles motor-controller team. It translated available shop hardware into a functional measurement system and created a practical way to estimate output power from speed and load data. While the brake system needed further refinement for longer-duration or higher-power testing, the project established a working foundation for motor validation and highlighted the key mechanical improvements needed in the next iteration.
