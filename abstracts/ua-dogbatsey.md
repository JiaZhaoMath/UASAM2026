---
speaker: Matthias Dogbatsey
role: student
campus: The University of Alabama
campus_short: UA
title: "A Diffuse-Interface Variational Implicit Solvation Model with the Size-Modified Poisson–Boltzmann Equation: Formulation, Numerical Computation, and Stern-Layer Formation"
slot: 3:40–4:00 p.m.
source: ../../abstracts/ua_dogbatsey_student.md
---

Diffuse-interface variational implicit solvation models (VISMs) enable efficient computation of ensemble average solvation energies without costly molecular dynamics sampling. However, the underlying coupled nonlinear PDEs remain computationally demanding, and the classical Poisson–Boltzmann model neglects finite ion size, predicting unphysically high concentrations near molecular surfaces. We present the first numerical realization of the diffuse-interface VISM, developed to date only analytically, and the first to incorporate steric effects via the fully nonlinear size-modified Poisson–Boltzmann (SMPB) equation, coupled to a p-Laplace equation that determines the solute-solvent interface variationally rather than prescribing it. Our solver combines an alternating direction implicit scheme with an inexact Newton–Krylov method, stabilized by a coupling relaxation strategy. We validate against manufactured solutions and biomolecular benchmarks, and show that both steric ion effects and short-range Lennard-Jones repulsion are required for a Stern layer to emerge.
