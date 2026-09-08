<!-- markdownlint-disable MD033 -->

<h1 align="left">
  The Mathematics and Physics of Reusable Launch Vehicles
</h1>

<p align="left">
  <strong>From the Rocket Equation to Propulsive Landing</strong>
</p>

<p align="left">
  A self-contained mathematical treatment of orbital launch, atmospheric re-entry,
  powered descent, and the economics of rocket reuse.
</p>

<p align="left">
  <a href="./main.pdf">
    <img alt="Read the paper" src="https://img.shields.io/badge/Paper-PDF-b31b1b?style=flat-square">
  </a>
  <a href="#citation">
    <img alt="Citation" src="https://img.shields.io/badge/cite-BibTeX-4c8cbf?style=flat-square">
  </a>
</p>

---

## About

Reusable launch vehicles turn a classical rocket-design problem into a coupled problem
in mass ratio, atmospheric flight, optimal control, structures, and economics.

This paper develops that problem from first principles and connects each result to
real launch systems, including **Falcon 9**, **Falcon Heavy**, **Starship / Super
Heavy**, **New Shepard**, **New Glenn**, **Electron**, and **Neutron**.

The treatment begins with the Tsiolkovsky rocket equation, derives staging and
recovery penalties, follows a booster through hypersonic entry and aerodynamic
control, and formulates the final landing burn as a real-time optimal-control problem.
Worked examples reproduce published Falcon 9 performance to within a few percent
using public vehicle data and elementary physics.

> **[Read the paper →](./main.pdf)**

## What is covered

- the rocket equation and the true delta-v cost of reaching low Earth orbit
- optimal staging and the payload penalty imposed by recovery propellant
- boostback, entry, and landing-burn requirements
- ballistic entry, dynamic pressure, convective heating, and grid-fin authority
- hoverslam guidance and powered descent through lossless convexification
- scaling laws explaining why reuse becomes more practical at larger vehicle sizes
- structural fatigue, engine life, landing loads, and multi-flight certification
- a cost-per-flight model and the conditions under which reuse breaks even
- first-principles case studies of current reusable launch systems

## Core relationships

The analysis is organized around a small set of governing relationships.

The ideal velocity increment follows from the Tsiolkovsky rocket equation:

$$
\Delta v = v_e \ln\left(\frac{m_0}{m_f}\right) = g_0 I_{sp}\ln\left(\frac{m_0}{m_f}\right).
$$

Orbital ascent adds gravity, drag, and steering losses:

$$
\Delta v_{\mathrm{required}} = v_{\mathrm{orbit}} + \Delta v_g + \Delta v_D + \Delta v_{\mathrm{steer}} - \Delta v_{\mathrm{rotation}}.
$$

For a reused booster, the economic objective becomes:

$$
\frac{C}{m_L} = \frac{C_B/N + C_R + C_U}{(1-\pi)m_{L,\mathrm{exp}}}.
$$

coupling flight count $N$, refurbishment cost $C_R$, and payload penalty
$\pi$ in a single measure of launch cost.

## Citation

If this work is useful in your research, please cite:

```bibtex
@article{gomez2026reusable,
  title   = {The Mathematics and Physics of Reusable Launch Vehicles:
             From the Rocket Equation to Propulsive Landing},
  author  = {Gomez, Kye},
  year    = {2026},
  month   = sep,
  note    = {Preprint},
  url     = {https://github.com/kyegomez/Reusable-Launch-Vehicles-Paper}
}
```

## Data note

Vehicle parameters are compiled from public manufacturer specifications, launch
webcasts, FAA environmental assessments, and conference publications. Values are
representative and may vary by vehicle block, mission, or source. The derivations
are the author's own.

## Author

**Kye Gomez** · [kye@swarms.world](mailto:kye@swarms.world)
