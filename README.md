# Signatures-of-PSGWs

These three files together compute the relative spectral energy density of primordial stochastic gravitational waves, GWs that originate from quantum fluctuations in the early universe.
The GWs are enhanced by inflation and become so large, that they cross the horizon. Outside the horizon their amplitudes remain constant as there is no causal contact anymore. At some point the horizon gets larger than the gravitational waves, with the large wavenumbers re-entering the horizon first. Once inside, the amplitude of teh GWs is changed due to the particles decoupling from the thermal bath. This is imprinted on the GWs and could potentially be measured by gravitational wave detectors.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)

## Installation
To run these files, you will need numpy, scipy, matplotlob and pandas.

## Usage

### SUSY
Start with the file [Entropy dof SM and SUSY.ipynb](https://github.com/annetkonings/Signatures-of-PSGWs/blob/main/Entropy%20dof%20SM%20and%20SUSY.ipynb). Here, the effective relativistic degrees of freedom of the particles in the Standard Model (SM) are calculated, as well as for the SUSY particles. In this extension of the SM, there is a supersymmetric particle 'cousin' for every SM particle. This means that every bosonic particle has a SUSY particle with a spin that differs by 1/2: i.e., a fermion. In the same way, every fermion has a SUSY particle that is a boson. Apart from the difference in spin, there is one more characteristic of SUSY particles that differentiates them from SM particles: their mass. Atlhough the exact values are unknown, their masses are theorised to be in the GeV - TeV range [^1].

The SM particles and their rest masses and number of helicity states are taken from the paper by Watanabe and Komatsu [^2].

### Decoupling

Neutrinos are a special case, as they do not decouple instantly. Therefore a sigmoid function is used to mimic a smooth transition from being coupled to the thermal bath, where Tν = Tγ, to decoupling, where Tν = (4/11)^(1/3)*Tγ. The energy range for this is taken as 1 < T < 3 MeV.



[^1]: Reference: M. Tanabashi et al., Review of Particle Physics, Phys. Rev. D 98, 030001 (2018).
[^2]: Reference: Y. Watanabe and E. Komatsu, Improved calculation of the primordial gravitational wave spectrum in the standard model, Physical Review D 73 (2006).
