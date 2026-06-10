# Multipartite Bell Multiport Probes

This repository contains the Mathematica notebook used for the numerical results in the paper **“Multipartite Bell inequalities with interferometric multiports.”**

The code implements fixed Fourier-generated probes for Bell scenarios of the form ((N,m,d)), where

* (N) is the number of parties,
* (m) is the number of measurement settings per party,
* (d) is the number of outcomes.

The notebook computes local deterministic bounds and numerical quantum values for Bell functionals written in the characteristic-function representation.

## Main file

notebooks/BellI_Nmd_fixed_fourier_probe.nb


This is the Mathematica notebook corresponding to the numerical analysis in the paper.

## What the code does

The notebook performs the following steps:

1. Constructs the fixed Fourier-generated probe (q_F^{(N,m,d)}).
2. Computes the local hidden-variable bound by maximizing over deterministic local strategies.
3. Optimizes the quantum value over shared quantum states and local multiport phase settings.
4. Computes the quantum-to-classical ratios for the real-part functional and the absolute-value witness.
5. Reproduces the numerical ratios reported in Table I of the paper.

## Output quantities

The main reported quantities are


R_Re  = Q_Re / C_Re
R_Abs = Q_Abs / C_Abs


where

* (C) is the local deterministic bound,
* (Q) is the best quantum value found numerically,
* (R) is the quantum-to-classical ratio.

## Notes

The optimization problems are nonconvex, so different runs may return different optimal states or phase parameters. However, the final Bell values and ratios should agree within numerical precision.

The fixed Fourier-generated probes are not claimed to be globally optimal or facet-defining Bell inequalities. They are structured probes adapted to the characteristic-function representation and the interferometric multiport measurement scheme.

## Requirements

The code requires Wolfram Mathematica / Wolfram Language.

## License

This code is released under the MIT License. See the `LICENSE` file for details.

