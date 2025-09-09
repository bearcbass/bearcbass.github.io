---
title: Fermi–Pasta–Ulam–Tsingou problem
seo_title: Fermi–Pasta–Ulam–Tsingou problem
summary: My final project for Foundations of Scientific Computing course, creating a simulation of the Fermi-Pasta-Ulam-Tsingou (FPUT) problem.
description: 
slug: Fermi–Pasta–Ulam–Tsingou
author: Sebastian Osorio

date: 2024-01-02T15:57:14-08:00
lastmod: 
expiryDate: 
publishDate: 

feature_image: fput_bead_schematic.png
feature_image_alt: schematic_fput_bead

project types:
  - Mathematical Computation

techstack:
  - Fortran
  - Python

live_url: 
source_url: "https://github.com/bearcbass/Fermi-Pasta-Ulam-Tsingou-Problem"

newsletter: false
---

My final project for Applied Mathematics 129: Foundations of Scientific Computing at the University of California, Santa Cruz was a simulation of the Fermi-Pasta-Ulam-Tsingou (FPUT) problem, demonstrating both its linear and nonlinear forms. The simulation models a chain of connected masses (like beads on a spring) using Leapfrog integration, tracking the motion of each mass over time and outputting the trajectories and parameters to study wave propagation and oscillatory dynamics in a 1D system.

In the simulation, the system is represented as a string of beads connected by springs, where each bead corresponds to a mass. When one or more beads are displaced, energy is initially localized in certain modes of the system. Over time, this energy spreads through the beads in a complex, often non-intuitive way, leading to oscillations that can appear almost chaotic. In the linear case, energy tends to distribute evenly among the beads, forming predictable wave patterns, while in the nonlinear case, the energy exhibits recurring behavior, concentrating back into the original modes after some time. This dynamic illustrates one of the surprising results of the FPUT problem: even in a seemingly simple system, nonlinear interactions can produce quasi-periodic energy transfers, rather than the complete thermalization one might expect.

### Animations

**String Motion with Displacement vs. Time plot:**
<img src="string_with_plot.gif" alt="FPUT string with plot" style="width:100%; max-width:1000px;">
