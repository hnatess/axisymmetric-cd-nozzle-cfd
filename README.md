# axisymmetric-cd-nozzle-cfd
1D sizing and CFD analysis of a variable-geometry axisymmetric convergent-divergent nozzle for a 6000 lbf-class turbofan engine.
# Axisymmetric C-D Nozzle Sizing and CFD Analysis

## Project Overview

This project focuses on the preliminary sizing and CFD-based evaluation of a variable-geometry axisymmetric convergent-divergent nozzle for a 6000 lbf-class low-bypass turbofan engine.

The main objective is to calculate the required throat area (A8) and exit area (A9) under different flight and engine operating conditions using one-dimensional compressible flow relations, transfer these values into a parametric nozzle geometry, and evaluate the resulting flow field using CFD simulations in ANSYS Fluent.

## Engineering Problem

A fixed-area nozzle may perform adequately at a single design point; however, turbofan engines operate over a wide range of off-design conditions. Therefore, the nozzle throat and exit areas must be evaluated across several operating points to avoid under-expansion, over-expansion, shock-related losses, and performance degradation.

This project investigates the required A8 and A9 variation for design and off-design conditions of a variable-geometry C-D nozzle.

## Methodology

The workflow consists of three main stages:

1. **One-dimensional gas-dynamic sizing**
   - Calculation of nozzle pressure ratio (NPR)
   - Choking condition check
   - Calculation of required throat area A8
   - Calculation of ideal exit Mach number
   - Calculation of expansion ratio A9/A8
   - Determination of required exit area A9

2. **Parametric geometry interpretation**
   - Conversion of area values into equivalent diameters
   - Identification of minimum and maximum throat/exit area limits
   - Interpretation of the nozzle opening envelope

3. **CFD analysis**
   - 3D steady compressible flow simulation
   - Ideal gas assumption
   - SST k-omega turbulence model
   - Local mesh refinement near the throat region
   - Inflation layers and y+ monitoring
   - Evaluation of Mach number, density, temperature and streamline contours

## Design and Off-Design Conditions

The reference design point was selected as:

- Altitude: 30,000 ft
- Flight Mach number: 0.8
- Inlet total pressure: 160 kPa
- Inlet total temperature: 750 K
- Outlet pressure: 30.090 kPa

Several off-design cases were also evaluated, including sea-level low power, sea-level maximum power, climb conditions, high-throttle high-altitude operation, high-NPR operation and low-power cruise.

## Tools Used

- ANSYS Fluent
- MATLAB / Excel
- CAD-based parametric geometry approach
- Compressible flow theory
- Mesh independence analysis

## Key Results

- The required throat area A8 and exit area A9 were calculated for design and off-design operating points.
- The design point and off-design cases showed different nozzle opening requirements due to changes in NPR, mass flow rate and total temperature.
- Mesh independence was evaluated using residual behavior, outlet Mach number, mass flow rate, outlet static pressure and wall y+.
- CFD results confirmed the expected choking behavior, post-throat acceleration and supersonic flow development in the divergent section.
- The one-dimensional sizing results showed good agreement with CFD trends in terms of exit Mach number and mass flow behavior.
- Density, temperature and streamline contours provided additional insight into compressibility effects, expansion behavior and local flow gradients.

## My Contributions

- Performed one-dimensional nozzle sizing calculations for A8, A9, NPR, expansion ratio and ideal exit Mach number.
- Prepared design and off-design operating point tables.
- Supported the transition from analytical sizing results to parametric nozzle geometry.
- Evaluated CFD results through Mach number, density, temperature and streamline contours.
- Interpreted mesh independence behavior using engineering output parameters rather than residuals alone.
- Contributed to the final technical report and presentation preparation.

## Project Status

Completed as a senior graduation project in Aircraft Engineering.

## Notes

This repository contains a summarized and portfolio-ready version of the graduation project. Large simulation files and full academic report files are not included.
