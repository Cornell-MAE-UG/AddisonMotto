---
layout: project
title: Senior Design Project
description: Class project 
summary: Developed and validated an optimized horizontal-axis wind turbine blade using BEM modeling, CFD, and wind-tunnel data.
order: 3
technologies: [MATLAB, ANSYS CFD]
image: /assets/images/senior_design_1.png
---

## Aerodynamic Blade Design Project

In this project, I developed a complete aerodynamic design and analysis workflow for a horizontal-axis wind turbine blade. Using CFD simulations in ANSYS Fluent, wind-tunnel data interpretation, and a MATLAB Blade Element Momentum (BEM) model, I evaluated baseline blade performance and designed an optimized geometry with improved efficiency at the target operating condition. The work involved generating chord and twist distributions based on optimal rotor theory, validating results across analytical, numerical, and experimental methods, and quantifying performance improvements through power-coefficient curves and Weibull-weighted annual energy production estimates. 

<h2 style="margin-top: 40px;">Performance & Blade Geometry Results</h2>

<p>
The following plots summarize aerodynamic performance predictions and the resulting optimized blade geometry. Comparisons between analytical BEM modeling, CFD simulations, and experimental wind-tunnel testing were used to validate the design approach and quantify efficiency improvements.
</p>

<div style="display: flex; flex-direction: column; align-items: center; gap: 45px; margin: 35px 0 10px 0;">

  <div style="text-align: center; width: 100%;">
    <img src="{{ "/assets/images/graph1.png" | relative_url }}"
         style="width: 100%; max-width: 800px; border-radius: 12px; border: 2px solid #222;">
    <p style="font-size: 13px; margin-top: 8px; color: #666;">
      Power coefficient versus tip-speed ratio comparing BEM predictions, CFD results, and wind-tunnel measurements, demonstrating improved efficiency near the target operating condition.
    </p>
  </div>

  <div style="text-align: center; width: 100%;">
    <img src="{{ "/assets/images/graph2.png" | relative_url }}"
         style="width: 100%; max-width: 800px; border-radius: 12px; border: 2px solid #222;">
    <p style="font-size: 13px; margin-top: 8px; color: #666;">
      Blade twist distribution along the span showing the optimized geometry designed to better align local aerodynamic loading with ideal rotor theory.
    </p>
  </div>

  <div style="text-align: center; width: 100%;">
    <img src="{{ "/assets/images/graph3.png" | relative_url }}"
         style="width: 100%; max-width: 800px; border-radius: 12px; border: 2px solid #222;">
    <p style="font-size: 13px; margin-top: 8px; color: #666;">
      Chord distribution comparison between the baseline and optimized blade, illustrating reduced material usage and improved aerodynamic efficiency across the span.
    </p>
  </div>

</div>

## Senior Design Project
<iframe 
  src="{{ site.baseurl }}/assets/senior_design.pdf"
  style="
    width:95%;
    max-width:1100px;
    aspect-ratio:9/8;
    height:auto;
    border:none;
    border-radius:0.75rem;
    background-color:#fff;
    box-shadow:0 2px 10px rgba(0,0,0,0.08);
    display:block;
    margin:0 auto 1rem auto;">
</iframe>

<div style="text-align:center;">
  <a href="{{ site.baseurl }}/assets/senior_design.pdf"
     target="_blank"
     style="font-size:1rem; text-decoration:none; color:#0077cc;">
     Download PDF →
  </a>
</div>



