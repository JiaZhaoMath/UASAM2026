---
speaker: Neethu Suma Raveendran
role: student
campus: University of Alabama at Birmingham
campus_short: UAB
title: CN–EMAC for Incompressible Flows with Parametric Uncertainty
slot: 1:30–1:50 p.m.
source: ../../abstracts/uab_Neethu-Suma-Raveendran-student.pdf
---

Accurate simulation of incompressible flows becomes particularly challenging when physical parameters are uncertain and the finite element velocity satisfies the incompressibility constraint only weakly. In this talk, we present a fully discrete Crank–Nicolson energy–momentum–angular-momentum conserving (CN–EMAC) finite element method for parameterized Navier–Stokes equations. It is coupled with stochastic collocation method, reducing the stochastic problem to independent deterministic solves at the collocation points.

We establish unconditional energy stability and derive a velocity error estimate of order O(h^k + Δt^2). For inviscid, unforced flow, the fully converged scheme without grad–div stabilization conserves kinetic energy, linear momentum, and angular momentum. Numerical experiments verify the predicted accuracy and demonstrate the method’s conservation properties and robustness for several benchmark flows.
