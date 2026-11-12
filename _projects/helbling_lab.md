---
layout: project
title: Helbling Robotics Research Lab
description: Gammabot brake development · Cornell Systems Engineering M.Eng.
summary: Developing a lightweight brake for Gammabot, with the assembly and flexure demonstrated in a benchtop test.
order: 2
technologies: [Mechanical Design, Prototyping, Experimental Testing]
image: /assets/images/helbling-gammabot-hardware.png
---

<figure class="lab-hero">
  <img src="{{ '/assets/images/helbling-gammabot-hardware.png' | relative_url }}" alt="Assembled Gammabot with electronics, wing mechanisms, and lightweight supporting frame" width="1162" height="1152" fetchpriority="high">
  <figcaption>Gammabot, the flapping-wing robot at the center of this project.</figcaption>
</figure>

## A brake for Gammabot

I’m developing a lightweight brake for **Gammabot**, a flapping-wing robot that moves along the water surface. Its wings drive it forward, but slowing down and holding position require another way to control its motion. My project brings together brake design, prototyping, and experiments to understand how a small mechanism can change the robot’s behavior on the water.

The challenge is balancing drag with weight: the brake needs to push against the water effectively while staying light enough for the robot. Longer term, better control of motion could help Gammabots pause and communicate through vibrations on the water surface.

## Actuation and assembly

The brake assembly and flexure are now working together in a benchtop test. The video below shows the mechanism moving before testing deployment in water.

The next step is to evaluate whether the brake enters the water reliably and how deployment affects the robot’s motion.

<figure class="lab-video lab-video-portrait">
  <video controls muted playsinline preload="metadata" poster="{{ '/assets/images/helbling-assembly-flexure-poster.jpg' | relative_url }}" aria-label="Benchtop test of the Gammabot brake assembly and flexure">
    <source src="{{ '/assets/videos/helbling-assembly-flexure.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support embedded video. <a href="{{ '/assets/videos/helbling-assembly-flexure.mp4' | relative_url }}">Watch the assembly and flexure test.</a>
  </video>
  <figcaption>Benchtop test of the brake assembly and flexure, November 2026.</figcaption>
</figure>

<details class="lab-previous-test">
  <summary>Earlier actuator-only test</summary>
<figure class="lab-video">
  <video controls playsinline preload="metadata" poster="{{ '/assets/images/helbling-actuator-poster.jpg' | relative_url }}" aria-label="Gammabot actuator motion demonstration">
    <source src="{{ '/assets/videos/helbling-actuator.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support embedded video. <a href="{{ '/assets/videos/helbling-actuator.mp4' | relative_url }}">Watch the actuator demonstration.</a>
  </video>
  <figcaption>Actuator motion before full-system assembly.</figcaption>
</figure>
</details>

<div class="lab-gallery">
  <figure>
    <a href="{{ '/assets/images/helbling-brake-assembly-cad.png' | relative_url }}"><img src="{{ '/assets/images/helbling-brake-assembly-cad.png' | relative_url }}" alt="CAD view of the brake mechanism within Gammabot’s frame" loading="lazy" width="1314" height="1022"></a>
    <figcaption>CAD of the brake integrated into the lightweight frame.</figcaption>
  </figure>
</div>

## Braking tests

Earlier trials used a low-friction magnetic guide rail and motion tracking to compare brake depths. Both the 2 mm and 5 mm configurations slowed the robot over a shorter distance than the no-brake baseline, as shown below.

One useful lesson came from deployment: an early pin-release approach disturbed the robot’s motion, and the brake sometimes struggled to break through surface tension. To isolate the braking effect, we ran these trials with the brake already lowered. The next experiments will test the complete deployment sequence.

<figure class="lab-results">
  <a href="{{ '/assets/images/helbling-brake-results.png' | relative_url }}"><img src="{{ '/assets/images/helbling-brake-results.png' | relative_url }}" alt="Normalized velocity versus distance: the 2 mm and 5 mm brake trials decay faster than the no-brake trials" loading="lazy" width="1932" height="1216"></a>
  <figcaption>Normalized velocity over distance for brake and no-brake trials. Select the plot to enlarge.</figcaption>
</figure>
