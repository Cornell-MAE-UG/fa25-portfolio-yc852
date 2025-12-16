---
layout: project
title: Turbine Blade
description: Probabilistic wind-turbine blade design and testing
technologies: MATLAB, Fusion 360, Wind-tunnel testing
image: assets/images/turbine-blade-cad.png
---

## Blade Design Project Overview

For MAE 4272, my team designed, manufactured, and tested a three‑bladed wind turbine optimized to maximize expected power output under a probabilistic wind environment while satisfying strict geometric, performance, and structural constraints.The blades were 3D‑printed in Accura 25 resin and mounted on a standardized hub with a magnetic particle brake, enabling controlled torque loading and power measurements in a wind tunnel. The design had to operate efficiently around the most probable wind speeds while staying within limits on blade radius, nacelle clearance, maximum RPM, torque‑brake capacity, and material strength.

## Design Approach

The team selected a NACA 4412 airfoil for its high lift‑to‑drag ratio at low Reynolds number and used a Weibull wind‑speed distribution (c = 5, k = 5) to define a design wind speed of about 5.05 m/s and a nominal design speed of 1000 RPM. Blade‑element modeling in MATLAB was used to set spanwise chord and twist so that each section operated near an optimal angle of attack of roughly 9.75 degrees, keeping torque below the 0.035 Nm brake limit and bending stresses well below the 55 MPa flexural strength of the resin (factor of safety ≈ 16.5).

## Testing and Results

In the wind tunnel, blades were tested over wind speeds of roughly 3.4–7.3 m/s, incrementally increasing brake voltage at each speed to build power‑versus‑RPM curves while enforcing RPM and safety limits. Torque was only increased during a run to avoid hysteresis effects, and steady‑state RPM, torque, voltage, and power were logged for each operating point. Experiments showed an optimal operating speed near 1050 RPM, very close to the prediction, but measured peak power was about 0.3 W versus a modeled 3.6 W, primarily due to mechanical losses (bearing and brake drag) and aerodynamic losses such as tip vortices, 3D effects, and surface roughness from 3D printing.

## Personal Contributions

My main contributions were in modeling, test planning, and data analysis. I implemented the blade‑element MATLAB model used to size the blade geometry and estimate torque, power, and bending stress, including the Weibull‑weighted expected power metric and comparison to the Accura 25 strength limit. I also co‑developed and refined the experimental protocol (RPM caps, hysteresis handling, and data‑logging steps) and led post‑processing of the power‑versus‑RPM curves to compare predictions with test data and identify dominant loss mechanisms.

## Selected Figures

- CAD rendering of the three‑bladed NACA 4412 rotor showing spanwise taper and twist. 

  <img src="/fa25-portfolio-yc852/assets/images/turbine-blade-cad.png"
       alt="Turbine blade CAD"
       style="max-width: 350px; height: auto;">
- Chord and pitch versus radius plot highlighting the near‑constant angle‑of‑attack design.

  <img src="/fa25-portfolio-yc852/assets/images/blade-chord-pitch.png"
       alt="Blade chord and pitch"
       style="max-width: 350px; height: auto;">
- Representative power‑versus‑RPM curve with probabilistic weighting at mid‑range wind speed.

  <img src="/fa25-portfolio-yc852/assets/images/power-curves.png"
       alt="Power curves"
       style="max-width: 350px; height: auto;">