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
After the Big Bang, the universe has high density and temperature and existing particle species are relativistic. All particles are in thermal (i.e., kinetic and chemical) equilibrium. We then get a period of inflation where the universe expands exponentially and the temperature decreases. From this point on, the reaction rates of elastic scattering (kinetic) and/or annihilation (chemical) of a particle species with the other particles in the thermal bath may become smaller than the Hubble expansion rate: Γ < H. Now they are no longer in thermal equilibrium. For thermal decoupling, Γ = n⟨σ​v⟩. Since the number density n depends on temperature as T^(3) for relativistic, and $T^{3/2}*\exp{-(mc^2)/(k_{B}*T)}$ for non-relaticvistic particles, the number densities get suppressed when the temperature decreases.
[^3][^4]
$\sqrt{3x-1}+(1+x)^2$


Neutrinos are a special case, as they do not decouple instantly. Therefore a sigmoid function is used to mimic a smooth transition from being coupled to the thermal bath, where Tν = Tγ, to decoupling, where $T_{\nu} = \big(\frac{4}{11}\big)^{1/3}T_{\gamma}$. The energy range for this is taken as 1 < T < 3 MeV. The difference in photon and neutrino temperature is because of electron-positron annihilation, effectively 'heating' the thermal bath after (most) neutrinos have already decoupled.
Photons decouple when the rate of free electron scattering drops below the expansion rate. After decoupling the photons free stream and can be observed as the cosmic microwave background.



[^1]: Reference: M. Tanabashi et al., Review of Particle Physics, Phys. Rev. D 98, 030001 (2018).
[^2]: Reference: Y. Watanabe and E. Komatsu, Improved calculation of the primordial gravitational wave spectrum in the standard model, Physical Review D 73 (2006).
[^3]: Reference: T. Bringmanna and S. Hofmannb, Thermal decoupling of WIMPs from first principles, Journal of cosmology and Astroparticle Physics, 2007(04):016, (2007).
[^4]: Reference: J. Schaye, J. Braspenning, E. Chaikin and R. Kugel, Lecture notes Origin and Evolution of the Universe, Leiden University (2022).
