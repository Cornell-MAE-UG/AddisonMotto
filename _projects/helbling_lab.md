---
layout: project
title: Helbling Robotics Research Lab
description: Gammabot brake development · Cornell Systems Engineering M.Eng.
summary: Developing a lightweight brake for Gammabot, with actuator motion demonstrated and full assembly underway.
order: 2
technologies: [Mechanical Design, Prototyping, Experimental Testing]
image: /assets/images/helbling-gammabot-hardware.png
---

I’m developing a lightweight brake for **Gammabot**, a flapping-wing robot that moves along the water surface. My work focuses on slowing the robot and integrating a mechanism to deploy the brake.

## Actuation and assembly

The actuator is moving, and I’m assembling the full system during the week of October 19, 2026. The next step is to test brake deployment on the assembled robot.

<figure class="lab-video">
  <video controls playsinline preload="metadata" poster="{{ '/assets/images/helbling-actuator-poster.jpg' | relative_url }}" aria-label="Gammabot actuator motion demonstration">
    <source src="{{ '/assets/videos/helbling-actuator.mp4' | relative_url }}" type="video/mp4">
    Your browser does not support embedded video. <a href="{{ '/assets/videos/helbling-actuator.mp4' | relative_url }}">Watch the actuator demonstration.</a>
  </video>
  <figcaption>Actuator motion before full-system assembly.</figcaption>
</figure>

<div class="lab-gallery">
  <figure>
    <a href="{{ '/assets/images/helbling-brake-assembly-cad.png' | relative_url }}"><img src="{{ '/assets/images/helbling-brake-assembly-cad.png' | relative_url }}" alt="CAD view of the brake mechanism within Gammabot’s frame" loading="lazy" width="1314" height="1022"></a>
    <figcaption>Brake assembly design.</figcaption>
  </figure>
  <figure>
    <a href="{{ '/assets/images/helbling-gammabot-hardware.png' | relative_url }}"><img src="{{ '/assets/images/helbling-gammabot-hardware.png' | relative_url }}" alt="Gammabot hardware with electronics mounted above the lightweight frame" loading="lazy" width="1162" height="1152"></a>
    <figcaption>Gammabot hardware.</figcaption>
  </figure>
</div>

## Braking tests

Earlier trials used a magnetic guide rail and motion tracking to compare brake depths. The 2 mm and 5 mm configurations showed faster velocity decay over distance than the no-brake baseline. These tests began with the brake already lowered; testing active deployment comes next.

<figure class="lab-results">
  <a href="{{ '/assets/images/helbling-brake-results.png' | relative_url }}"><img src="{{ '/assets/images/helbling-brake-results.png' | relative_url }}" alt="Normalized velocity versus distance: the 2 mm and 5 mm brake trials decay faster than the no-brake trials" loading="lazy" width="1932" height="1216"></a>
  <figcaption>Normalized velocity over distance for brake and no-brake trials. Select the plot to enlarge.</figcaption>
</figure>
